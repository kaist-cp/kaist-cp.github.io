{% for paper in site.data.papers %}
{% if include.author_id == null or paper.authors contains include.author_id %}
{% if include.tag == null or paper.tags contains include.tag %}
{% if include.submitted or paper.submitted == null %}

{% assign author_links = "" | split: "" %}
{% for author_id in paper.authors %}

  {% capture link %}{% include person_link.md person_id=author_id %}{% endcapture %}
  {% assign link = link | strip %}

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
  {% if paper.website %}\[[project page](/{{ paper.website }})\]{% endif %} ​
  {% if paper.copy_publisher %}\[[publisher's page]({{ paper.copy_publisher }})\]{% endif %} ​
  <br />
  {% if include.abstract and paper.abstract %}
  <p style="margin: 20px; font-size: 0.9em; line-height: 1.44em;"><b>Abstract</b>: {{ paper.abstract }}</p>
  <br />
  {% endif %}
{% endif %}
{% endif %}
{% endif %}
{% endfor %}
