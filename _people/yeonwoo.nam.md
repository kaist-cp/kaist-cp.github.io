layout	title	excerpt
page
Yeonwoo Nam (남연우)
Yeonwoo Nam's website
{%- assign person_id = "janggun.lee" %} {%- assign person = site.data.people | where:"id",person_id | sample %}

I am a Undergraduate Student at KAIST department of Mathematical Sciences and School of Computing. I am interested in formal verification of concurrent systems.

{% include person_contact.md person_id=person_id %}

{% include person_education.md person_id=person_id %}
