
{% assign categories = site.data.skills.technical %}
{% for category in categories -%}
#### {{ category[0] | replace: "_", " " | capitalize }}

| Skill | Level |
| ----- | ----- |
{% for skill in category[1] -%}
| {{ skill.title }} | {{ skill.level }} |
{% endfor %}
{% endfor %}

---

### Soft Skills

| Skill | Level |
| ----- | ----- |
{% for skill in site.data.skills.soft -%}
| {{ skill.title }} | {{ skill.level }} |
{% endfor %}
