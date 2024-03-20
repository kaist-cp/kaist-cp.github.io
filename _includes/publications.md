<style>
p.abstract-paragraph {
  margin-bottom: 0rem;
  text-align: justify;
  text-justify: inter-word;
}
/* https://stackoverflow.com/questions/60980466/dont-indent-first-line-of-first-paragraph-using-css */
p.abstract-paragraph + p.abstract-paragraph {
  text-indent: 2em;
}
</style>

{% for paper in site.data.papers %}
{% if include.author_id == null or paper.authors contains include.author_id %}
{% if include.tag == null or paper.tags contains include.tag %}
{% if include.submitted or paper.submitted == null %}

<!-- Set authors -->
{% assign author_links = "" | split: "" %}
{% for author_id in paper.authors %}

  {% capture link %}{% include person_link.md person_id=author_id %}{% endcapture %}
  {% assign link = link | strip %}

  {% if include.author_id == author_id %}
    {% assign link = "**" | append: link | append: "**" %}
  {% endif %}

  {% if paper.cofirst_authors contains forloop.index %}
    {% assign link = link | append: "†" %}
  {% endif %}

  {% assign author_links = author_links | push: link %}
{% endfor %}

<!-- Set paper copies -->
{% assign paper_links = "" | split: "" %}
{% if paper.doi %}
  {% assign link = "[doi](https://doi.org/" | append: paper.doi | append: ")" %}
  {% assign paper_links = paper_links | push: link %}
{% endif %}
{% if paper.handle %}
  {% assign link = "[handle](https://hdl.handle.net/" | append: paper.handle | append: ")" %}
  {% assign paper_links = paper_links | push: link %}
{% endif %}
{% if paper.copy_local %}
  {% assign link = "[local](" | append: paper.copy_local | append: ")" %}
  {% assign paper_links = paper_links | push: link %}
{% endif %}

<!-- Set artifacts -->
{% assign artifact_links = "" | split: "" %}
{% for artifact in paper.artifact_local %}
  {% assign link = "[" | append: artifact.name | append: "](" | append: artifact.url | append: ")" %}
  {% assign artifact_links = artifact_links | push: link %}
{% endfor %}

- <span style="font-size: 110%; font-weight: bold;">({% if paper.venue_short %}{{ paper.venue_short }} {% endif %}{{ paper.year }})</span>
  <span style="font-size: 110%; font-weight: bold;">{{ paper.title }}.</span>
  <br />
  {{ author_links | join: ", " }}{% if paper.cofirst_authors %} (†: co-first authors in alphabetical order){% endif %}.
  <br />
  {{ paper.venue }}{% if paper.status %} ({{ paper.status }}){% endif %}.
  <br />
  {% if paper_links.size > 0 %}\[paper: {{ paper_links | join: ", " }}\] {% endif %} ​
  {% if artifact_links.size > 0 %}\[artifact: {{ artifact_links | join: ", " }}\] {% endif %} ​
  {% if include.website and paper.website %}\[[website]({{ paper.website }})\]{% endif %} ​
  <br />
  {% if include.full and paper.abstract %}
  <div style="margin: 20px; font-size: 0.9em; line-height: 1.44em;">
    <b>Abstract</b>
    {% assign paragraphs = paper.abstract | newline_to_br | strip_newlines | split: '<br />' %}
    {% for paragraph in paragraphs %}<p class="abstract-paragraph">{{ paragraph }}</p>{% endfor %}
  </div>
  {% endif %}
  {% if include.full and paper.changelog %}
  <div style="margin: 20px; font-size: 0.9em; line-height: 1.44em;">
    <b>Changelog/Errata</b>
    <ul>
    {% for change in paper.changelog %}
      <li> {{ change }} </li>
    {% endfor %}
    </ul>
  </div>
  {% endif %}
{% endif %}
{% endif %}
{% endif %}
{% endfor %}
