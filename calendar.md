---
layout: default
title: Calendar
nav_weight: 2
---

## {{ page.title }}

The calendar is subject to change over the course of the semester.

<div class="classplan">

{% assign calendar = site.data.calendar | sort: 'date' %}
<table>
<thead>
     <tr>
       <th style="text-align: left">Date</th>
       <th style="text-align: left">Topic</th>
       <th style="text-align: left">Comments</th>
     </tr>
</thead>
<tbody>

{% for item in calendar %}
<tr>
<td>{{ item.date | date: "%a %-d %b" }}</td>
<td>{{ item.topic | markdownify | strip | remove:'<p>' | remove: '</p>' }}</td>
<td>{{ item.comments | markdownify | strip | remove:'<p>' | remove: '</p>' }}</td>
</tr>
{% endfor %}

</tbody>
</table>

</div>
