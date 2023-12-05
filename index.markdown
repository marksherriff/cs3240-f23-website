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
- Monday, Dec 11 :: Project Demos and Student Conferences begin - [Sign Up For An Appointment](https://outlook.office.com/bookwithme/user/165022bfe47740ca8bb1433bd8759a7d@virginia.edu/?getrequesturl=https%3a%2f%2foutlook.office.com%2fows%2fOID%3a49dcef75-2418-4f39-a2fb-a00ea100a06b%407b3480c7-3707-4873-8b77-e216733a65ac%2fbeta%2fBookWithMe%2fCheckBookable%3fbookingcode%3d14e042c2-b52c-4917-a015-036f2e228210%26itemid%3dRUxr961gK0iv3Nw9w2fBtg2%26authtoken%3deyJhbGciOiJSUzI1NiIsImtpZCI6IloyeTkxSDI2NlFTcTVySGR2K1ljUFRxUVVzTT0iLCJ0eXAiOiJKV1QiLCJ4NXQiOiJNTkVPUHc1MEpXTk11NFBjT0ZFaTVYVW9ralUifQ.eyJvaWQiOiI0OWRjZWY3NS0yNDE4LTRmMzktYTJmYi1hMDBlYTEwMGEwNmIiLCJ2ZXIiOiJSZXNvdXJjZUxvb3BiYWNrLlVzZXIuVjEiLCJzY3AiOiJPcGVuQm9vay1JbnRlcm5hbC5SZWFkV3JpdGUiLCJyc2NvcGVsZW4iOiIyMTgiLCJyZXNvdXJjZV9zY29wZSI6IntcIlVSTFwiOlwiZXZVdXlDYTNvN2s3K3FZMTZKRFliK0RiMm0yZWFxaDJzcXJiekJtUkNBND1cIn0iLCJjb3JyaWQiOiIwZTQ3ZTM2MC04YmViLTRiZmUtYjRiNi1mNzliNTc1NDc5NDEiLCJhcHBpZCI6IjE1N2NkZmJmLTczOTgtNGE1Ni05NmMzLWU5M2U5YWIzMDliNSIsImFwcGlkYWNyIjoiMCIsInRpZCI6IjdiMzQ4MGM3LTM3MDctNDg3My04Yjc3LWUyMTY3MzNhNjVhYyIsImlhdCI6MTcwMTc5MDgxNywibmJmIjoxNzAxNzkwODE3LCJleHAiOjE3MDk1NjY4MTcsImlzcyI6Imh0dHBzOi8vcmVzb3VyY2Uuc2VsZi8iLCJhdWQiOiJodHRwczovL291dGxvb2sub2ZmaWNlLmNvbSJ9.yCQnkj56Vgs9xs0-BX3uEq965SAZh4J1pxjBwie9nwFSb1_uoYcBrvFqc-AgC0vqQ9dfxL_Yd5lTQOEifL2XPGPuUklv3y9cNlQeCLmfOKzzAqVmEqjMRdTeEc9gxa37g1ydemB5Cuo_hPeungXZoeLD6aJqLTk0y4bszPUilKyw0gYEeF5ujkuIOJRppwsG4x5TEIXC2NUuxM4pvQ-CnJcVXzLzpodB0lNGnAVDUxqh7FbahV0B0iYOUfQD09GOWhlwXnZJAiYM88LpcpOHNZ-b8vLeTuw97LJDIivkNPRdNBFv4jBkgQaQZooxl_KzYUpT0OWCpa-CUUyCFzMQrA&anonymous&ep=mlink)
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