---
layout: default
title: Schedule
nav_order: 3
---

# Course Schedule
{: .no_toc }
__Currently under construction!  Nothing here is finalized!__

_NOTE: Schedules are subject to change.  Watch this page for updates!_

1. TOC
{:toc} 

## Lecture Schedule

<table class="schedtab"><thead>
<tr>
    <th>Date</th>
    <th>Topic</th>
    <th>Due Dates</th>
    </tr>
    </thead>
    <tbody>
{% for day in site.data.lectureschedule %}
{% if day.type == 'holiday' %}
<tr class="holiday">
{% elsif day.type == 'quiz' %}
<tr class="quiz">
{% else %}
<tr>
{% endif %}
<td class="text-center sched">{{day.date}}</td>
<td class="sched">
{% if day.coursepack %}
<a href="{{day.coursepack}}">
{% endif %}
{{day.topic}}
{% if day.coursepack %}
    </a>
{% endif %}
{% if day.lectures or day.readings %}
<br><span class="sched-sub">
    {% if day.readings %}
    Readings:
    {% for read in day.readings %}
    <a href="{{read.link}}">{{read.topic}}</a> 
    {% endfor %}
    {% endif %}
    {% if day.lectures and day.readings %}
    -
    {% endif %}
    {% if day.lectures %}
    Slides:
    {% for pdf in day.lectures %}
    {% if pdf.link %}
    <a href="{{pdf.link}}" alt="{{pdf.alt}}">{{pdf.time}}</a> 
    {% else %}
    <span title="{{pdf.alt}}">{{pdf.time}}</span> 
    {% endif %}
    {% endfor %}
    {% endif %}
    </span>
{% endif %}
</td>
<td class="sched">{{day.notes}}</td>
</tr>
{% endfor %}
</tbody></table>

## Project Schedule

<table class="schedtab"><thead>
<tr>
    <th>Week Of</th>
    <th>Weekly Objective</th>
    <th>Sprint</th>
    </tr>
    </thead>
    <tbody>
{% for day in site.data.labschedule %}
{% if day.type == 'holiday' %}
<tr class="holiday">
{% elsif day.type == 'quiz' %}
<tr class="quiz">
{% else %}
<tr>
{% endif %}
<td class="text-center sched">{{day.date}}</td>
<td class="sched">
{% if day.coursepack %}
<a href="{{day.coursepack}}">
{% endif %}
{{day.topic}}
{% if day.coursepack %}
    </a>
{% endif %}
{% if day.lectures or day.readings %}
<br><span class="sched-sub">
    {% if day.readings %}
    Readings:
    {% for read in day.readings %}
    <a href="{{read.link}}">{{read.topic}}</a> 
    {% endfor %}
    {% endif %}
    {% if day.lectures and day.readings %}
    -
    {% endif %}
    {% if day.lectures %}
    Slides:
    {% for pdf in day.lectures %}
    {% if pdf.link %}
    <a href="{{pdf.link}}" alt="{{pdf.alt}}">{{pdf.time}}</a> 
    {% else %}
    <span title="{{pdf.alt}}">{{pdf.time}}</span> 
    {% endif %}
    {% endfor %}
    {% endif %}
    </span>
{% endif %}
</td>
<td class="sched">{{day.notes}}</td>
</tr>
{% endfor %}
</tbody></table>

## Office Hours Calendar

<iframe src="https://calendar.google.com/calendar/embed?src=n0peik670v06jh9bfb0js1k1k8%40group.calendar.google.com&ctz=America%2FNew_York&mode=WEEK" style="border: 0" width="100%" height="600" frameborder="0" scrolling="no"></iframe>