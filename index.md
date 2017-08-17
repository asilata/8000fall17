---
layout: default
nav_title: Course home
nav_weight: 1
---

<div id="about">

<div>
## Announcements
<ul>
{% for post in site.posts limit: 3%}
<li>
<strong>{{ post.date | date: "%a %b %-d" }}:</strong> {{ post.content | remove: '<p>' | remove: '</p>'}}
</li>
{% endfor %}
</ul>
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

## Homeworks

{% assign homeworks = site.data.homeworks | sort: 'due' %}
{% for hw in homeworks %}
* [{{ hw.name }}]({{ hw.link }}) (due on {{ hw.due | date:"%A" }}, {{ hw.due | date:"%B %-d"}})
{% endfor %}

