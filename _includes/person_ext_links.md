{%- assign person_id = include.person_id %}
{%- assign person = site.data.people | where:"id",person_id | sample %}

<ul class="list-inline">
  <li class="list-inline-item">
    <a href="{{ person_url }}">:house:</a>
  </li>

  <li class="list-inline-item">
    <a href="mailto:{{ mail_id }}@kaist.ac.kr">:love_letter:</a>
  </li>

  {% if person.twitter %}
  <li class="list-inline-item">
    <a href="https://twitter.com/{{ person.twitter }}"><i class="fa fa-twitter"></i></a>
  </li>
  {% endif %}

  {% if person.github %}
  <li class="list-inline-item">
    <a href="https://github.com/{{ person.github }}">
      <img class="emoji" title=":octocat:" alt=":octocat:" src="https://github.githubassets.com/images/icons/emoji/octocat.png" height="20" width="20">
    </a>
  </li>
  {% endif %}

  {% if person.orcid %}
  <li class="list-inline-item">
    <a href="https://orcid.org/{{ person.orcid }}"><img class="orcid" style="width: 20px; " src="{{ '/assets/images/orcid.svg' | relative_url }}"></a>
  </li>
  {% endif %}

  {% if person.dblp %}
  <li class="list-inline-item">
    <a href="{{ person.dblp }}"><img class="dblp" style="width: 20px; " src="{{ '/assets/images/dblp.png' | relative_url }}"></a>
  </li>
  {% endif %}

  {% if person.google_scholar %}
  <li class="list-inline-item">
    <a href="{{ person.google_scholar }}"><img class="google" style="width: 20px; " src="{{ '/assets/images/google.png' | relative_url }}"></a>
  </li>
  {% endif %}

  {% if person.keybase %}
  <li class="list-inline-item">
    <a href="https://keybase.io/{{ person.keybase }}"><img class="keybase" style="width: 20px; " src="{{ '/assets/images/keybase.png' | relative_url }}"></a>
  </li>
  {% endif %}
</ul>
