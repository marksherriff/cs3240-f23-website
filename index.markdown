---
layout: default
title: Home
nav_order: 1
description: "CS 3240 - Advanced Software Development Techniques"
permalink: /
---

# CS 3240 - Fall 2023
## Advanced Software Development Techniques
_aka Software Engineering_

[Online Coursepack]({{ site.data.externallinks.coursepack }}){: .btn  .btn-primary .mr-2 }
[Gradescope]({{ site.data.externallinks.gradescope }}){: .btn .btn-primary .mr-2  }
[Piazza]({{ site.data.externallinks.piazza }}){: .btn .btn-primary .mr-2  }
[Collab]({{ site.data.externallinks.lms }}){: .btn .btn-primary .mr-2  }
[GitHub]({{ site.data.externallinks.github_organization }}){: .btn .btn-primary .mr-2  }

## Lecture and Lab Sessions
{% for section in site.data.semesterinfo.lecture_sections %} {{ section }}    
{% endfor %}   
## Staff Information

{% for professor in site.data.professors %}

__Instructor:__ {{ professor.name }}   
Office: {{ professor.office }}   
Office Hours: {{ professor.office_hours }}        
Email: [{{ professor.email }}]({{ professor.email }})   
Website: [{{ professor.website }}]({{ professor.website }})   

{% endfor %}

__Teaching Assistants:__ {% for ta in site.data.tas %} {{ ta.name }}, {% endfor %}  