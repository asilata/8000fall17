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
| Problem session | TBA                                                                        |
| Instructor      | [Asilata Bapat](https://asilata.github.io/) (`asilata` at `uga` dot `edu`) |
| Office hours    | TBA in Boyd 605                                                            |
| Grader          | TBA                                                                        |

</div>


</div>

## Lecture notes
The latest version of the lecture notes is available [here](https://www.overleaf.com/read/rfcvwktkdtzn).
The LaTeX class used has been adapted from [this one](http://blog.poormansmath.net/latex-class-for-lecture-notes/).

