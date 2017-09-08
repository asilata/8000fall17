---
layout: default
nav_title: Course home
nav_weight: 1
---

<div id="about">

<div>
## Latest announcements
<ul>
{% for post in site.posts limit: 3%}
<li>
<strong>{{ post.date | date: "%a %b %-d" }}:</strong> {{ post.content | remove: '<p>' | remove: '</p>'}}
</li>
{% endfor %}
</ul>
</div>

<div class="classinfo">

| Lectures        | TR 11:00am to 12:15pm, Boyd 326                                                                     |
| Problem session | T 4:30pm to 5:30pm in Boyd 628                                                                      |
| Instructor      | [Asilata Bapat](https://asilata.github.io/) (`asilata` at `uga` dot `edu`)                          |
| Office hours    | M 2:00pm to 3:00pm and T 3:30pm to 4:30pm  in Boyd 605                                              |
| Graders         | David Galban (`dmg30956` at `uga` dot `edu`)<br/>Arvind Suresh (`arvind.suresh25` at `uga` dot `edu`)<br/>Makoto Suwama (`makoto.suwama25` at `uga` dot `edu`) |

</div>


</div>

## Lecture notes
The latest version of the lecture notes is available [here](https://www.overleaf.com/read/rfcvwktkdtzn).
The LaTeX class used has been adapted from [this one](http://blog.poormansmath.net/latex-class-for-lecture-notes/).

## Homeworks

{% assign homeworks = site.data.homeworks | sort: 'due' %}
<ul>
{% for hw in homeworks %}
<li>
<a href="{{ hw.link }}">{{ hw.name }}</a> (due on {{ hw.due | date:"%A" }}, {{ hw.due | date:"%B %-d"}})
</li>
{% endfor %}
</ul>

## Older announcements
<ul>
{% for post in site.posts offset: 3%}
<li>
<strong>{{ post.date | date: "%a %b %-d" }}:</strong> {{ post.content | remove: '<p>' | remove: '</p>'}}
</li>
{% endfor %}
</ul>
