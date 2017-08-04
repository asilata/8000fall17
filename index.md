---
layout: default
nav_title: Course home
nav_weight: 1
---

<div id="about">

<div>
## Announcements
{% for post in site.posts %}
* **{{ post.date | date: "%a %b %-d" }}:** {{ post.content | remove: '<p>' | remove: '</p>'}}
{% endfor %}
</div>

<div class="classinfo">

| Lectures        | TR 11:00am to 12:15pm, Boyd 326                                            |
| Problem session | M 11:15am to 12:05pm, Boyd 326                                             |
| Instructor      | [Asilata Bapat](https://asilata.github.io/) (`asilata` at `uga` dot `edu`) |
| Office hours    | TBA in Boyd 605                                                            |
| Grader          | TBA                                                                        |

</div>


</div>
