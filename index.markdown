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
Our course is structured around understanding the different aspects of the software development lifecycle.  During this course, students will learn to elicit and model software requirements, choose from various design options for a solution, implement a large software system in teams using a modified Scrum methodology, perform quality assurance, and learn about ethical and professional issues, such as diversity issues, how to handle data responsibly, and software licensing.

[Online Coursepack]({{ site.data.externallinks.coursepack }}){: .btn  .btn-primary .mr-2 }
[Gradescope]({{ site.data.externallinks.gradescope }}){: .btn .btn-primary .mr-2  }
[Piazza]({{ site.data.externallinks.piazza }}){: .btn .btn-primary .mr-2  }
[Canvas]({{ site.data.externallinks.lms }}){: .btn .btn-primary .mr-2  }
[GitHub]({{ site.data.externallinks.github_organization }}){: .btn .btn-primary .mr-2  }

## End of Semester Information
- Monday, Dec 4 :: [Final Exam Signup Available](https://docs.google.com/forms/d/e/1FAIpQLSe0bOUDRFxxMpks0IebgulAQpB5P4B9YTlK-4QNYRprLnEssQ/viewform?usp=sf_link) & Quiz 3 Score Returned
- Tuesday, Dec 5 :: Quiz 3 Regrade Requests close at 9:30 AM EST & Final Lecture Session with [Sherriff's AMA (Ask Me Anything)](https://docs.google.com/forms/d/e/1FAIpQLSc-vWjpIuPjGaRXRkjPS9UjhmZtG7BIk42LENhQRbFNDtYwgQ/viewform?usp=sf_link)
- Wednesday, Dec 6 :: All remaining grades returned
- Thursday, Dec 7 :: Signup for the 2:00 Exam closes at 11:00 AM, then 2:00 Exam in Rice 130
- Monday, Dec 11 :: Project Demos and Student Conferences begin as needed
- Thursday, Dec 14 :: Signup for the Friday Exam closes at 12:00 Noon
- Friday, Dec 15 :: Exam at 9:00 in Rice 130
- Sunday, Dec 17 :: Grades submitted to SIS

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