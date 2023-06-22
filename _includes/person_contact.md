{%- assign person_id = include.person_id %}
{%- assign person = site.data.people | where:"id",person_id | sample %}

{% if person.kaist_id %}
{% assign mail_id = person.kaist_id %}
{% else %}
{% assign mail_id = person.id %}
{% endif %}

#### Contact

- :love_letter: Email: [{{ mail_id }}@kaist.ac.kr](mailto:{{ mail_id }}@kaist.ac.kr)
- :octocat: GitHub: [{{ person.github }}](https://github.com/{{ person.github }})
- :page_facing_up: Bibliography:{% if person.orcid %} <a href="https://orcid.org/{{ person.orcid }}"><img class="orcid" style="width: 20px; " src="{{ '/assets/images/orcid.svg' | relative_url }}"> ORCID</a>, {% endif %}
  <a href="{{ person.dblp }}"><img class="dblp" style="width: 20px; " src="{{ '/assets/images/dblp.png' | relative_url }}"> DBLP</a>,
  <a href="{{ person.google_scholar }}"><img class="google" style="width: 20px; " src="{{ '/assets/images/google.png' | relative_url }}"> Google Scholar</a>
- :office: Place: {{ person.place }}
{% if person.keybase %}- :key: PGP key (<img class="keybase" style="width: 20px; " src="{{ '/assets/images/keybase.png' | relative_url }}"> keybase): [{{ person.keybase }}](https://keybase.io/{{person.keybase}}){% endif %}
