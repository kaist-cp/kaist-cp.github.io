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

{% assign author_links = "" | split: "" %}
{% for author_id in paper.authors %}

  {% capture link %}{% include person_link.md person_id=author_id %}{% endcapture %}
  {% assign link = link | strip %}

  {% if include.author_id == author_id %}
    {% assign link = "**" | append: link | append: "**" %}
  {% endif %}

  {% if paper.cofirst_authors contains forloop.index %}
    {% assign link = link | append: "\*" %}
  {% endif %}

  {% assign author_links = author_links | push: link %}
{% endfor %}

- <span style="font-size: 110%; font-weight: bold;">({% if paper.venue_short %}{{ paper.venue_short }} {% endif %}{{ paper.year }})</span>
  <span style="font-size: 110%; font-weight: bold;">{{ paper.title }}.</span>
  <br />
  {{ author_links | join: ", " }}{% if paper.cofirst_authors %} (\*: co-first authors in alphabetical order){% endif %}.
  <br />
  {{ paper.venue }}{% if paper.status %} ({{ paper.status }}){% endif %}.
  <br />
  {% if paper.copy_local %}\[[paper]({{ paper.copy_local }})\]{% endif %} ​
  {% if paper.artifact_local %} ​
    {% for artifact in paper.artifact_local %} ​
      \[[artifact \({{ artifact.name }}\)]({{ artifact.url }})\] ​
    {% endfor %} ​
  {% endif %} ​
  {% if include.website and paper.website %}\[[project page](/{{ paper.website }})\]{% endif %} ​
  {% if paper.copy_publisher %}\[[publisher's page]({{ paper.copy_publisher }})\]{% endif %} ​
  <br />
  {% if include.abstract and paper.abstract %}
  <div style="margin: 20px; font-size: 0.9em; line-height: 1.44em;">
    <b>Abstract</b>
    {% assign paragraphs = paper.abstract | newline_to_br | strip_newlines | split: '<br />' %}
    {% for paragraph in paragraphs %}<p class="abstract-paragraph">{{ paragraph }}</p>{% endfor %}
  </div>
  {% endif %}
{% endif %}
{% endif %}
{% endif %}
{% endfor %}
