{%- assign person_id = include.person_id %}
{%- assign person = site.data.people | where:"id",person_id | sample %}


#### Experience

{% for experience in person.experiences %}
- {{ experience }}
{% endfor %}
