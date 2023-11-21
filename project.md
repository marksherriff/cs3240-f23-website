---
layout: default
title: Project Information
nav_order: 4
---

# Project Information
{: .no_toc }

## Table of Contents
{: .no_toc .text-delta }

1. TOC
{:toc}

## Project Options and Requirements

Your team must choose one of these project options.  You have a great deal of agency within these options, but you must stick to the core use cases of the project.

You __must__ meet any common and project specific requirements listed below.

## Common Requirements

All projects must do the following, regardless of idea chosen:

* All projects must incorporate Google user accounts as the primary way that someone logs into the system.  You will need to use the Google account API to make this work.  There are several libraries that are built for Django to work with Google accounts with tutorials.
* You will have to create two different user access levels for each project.  This will take a slightly different form with each project, but the basic idea is some users will be “common” users and some users will be “administrative” users.  Users of one type _should not_ be able to access features of the other type!
* The two test accounts we will use will be: common user - cs3240.student@gmail.com and admin user - cs3240.super@gmail.com
* All projects must incorporate the Google Maps Javascript API - [https://developers.google.com/maps/documentation/javascript](https://developers.google.com/maps/documentation/javascript).  How you implement it and utilize it is up to your team, within reason.
* All projects must be built using the prescribed language (Python 3), framework (Django 4), build environment (GitHub Actions CI), source control management (GitHub), and cloud hosting (Heroku).  No exceptions to these will be granted.
* All projects must use the PostgreSQL database engine for production on Heroku and continuous integration (on GitHub Actions).  You are allowed to use SQLite for local testing so you do not have to install PostgreSQL on your own machine, but another option is to change your `settings.py` file point to the PostgreSQL DB on Heroku at all times.  

## Project Options

These are the _base_ requirements for your projects and are here to ensure that all three projects are of basically the same complexity.  Projects that only complete these features will not earn much XP.  You will add more use cases for both the student and admin users during your requirements elicitation activities.

### Project Domain 1: Hidden Locations
{: .no_toc }

Projects in this domain will in some way "hide" locations from users and encourage them to find them.  One prominent example is geocaching (example information at [https://www.geocaching.com/play](https://www.geocaching.com/play)).  There are other things you could do in this category as well, including puzzle hunts or other surprises.  Some optional features that you may add include leaderboards, user comments, and much more.  For this domain, regular users should be able to "do the hunt" for the locations and can submit their own hunts/locations for others to find.  However, these additions SHOULD NOT appear until an administrative user logs in and approves the submission.  Once it is approved, it can appear for everyone.  Administrators can also deny submissions, sending a reason along with it to the user in the app (not outside the app via email, etc.).

### Project Domain 2: Known Locations
{: .no_toc }

Projects in this domain will make locations known to users up front as a way to help guide them or find something around Grounds.  Some examples include points of interest for incoming first years, the best places on Grounds to go for a run, or historic locations.  Keep your app focused on guiding the users and don't try to add a lot of "other" functionality.  Something like rating a location or leaving comments is fine.  Adding a feature schedule a time to meet someone at a location is too much.  For this domain, regular users should be able to propose new locations and can submit their own locations to be added to the app's database.  However, these additions SHOULD NOT appear until an administrative user logs in and approves the submission.  Once it is approved, it can appear for everyone.  Administrators can also deny submissions, sending a reason along with it to the user in the app (not outside the app via email, etc.).

## Team Roles

Each member of your five person team will take on one of these roles.  Each role has different responsibilities, but ALL ROLES require that you be an active contributor to the code of the project.  In other words, if you take on Scrum Master, that doesn't mean you don't have to contribute as much code as someone else.  Please see the [information on Assessment and Grading](/syllabus.html#assessment-and-grading) for more information.

__Scrum Master__ - The Scrum Master could also be called the Team Leader, but it's not really a "leader" position, per se, in that they are not making major decisions about the project itself.  The Scrum Master is responsbile for keeping everyone on track, facilitating all team meetings, and monitoring team status / issues.  The course staff will come to the Scrum Master first if there are any team issues or questions, and similarly the Scrum Master needs to know what's going on with the team and can communicate with the staff if someone is falling behind, etc.

* Reasons to be the Scrum Master: You like keeping schedules; you like keeping things organized; you don't mind being the point of contact with the staff.
* Reasons not to be the Scrum Master: You are not the most organized person; you don't think you can stay on top of what the team is working on; you don't like talking to the staff.

_Major Artifact_: [Scrum Master Final Report]({{ site.data.externallinks.scrum_master_report_template }}), due at the end of the semester   

__Requirements Manager__ - The Requirements Manager is responsible for keeping up with the features of the project.  This person will take the lead on the requirements elicitation process (which takes place in the first couple weeks of the project) as their major activity.  Note that the Requirements Manager doesn't do the whole process - they just lead the effort.  Everyone else has to participate as well!  Then throughout the semester they will manage the feature/issue tracker in GitHub, monitoring the state of the project.

* Reasons to be the Requirements Manager: You are interested in learning how requirements are created; you want to find out what your fellow stduents are excited about with your project; you like updating a spreadsheet; you like knowing "what's coming next" in the project.
* Reasons to not be the Requirements Manager: You have no interest in interacting with other people to find out what they want in a system; your first couple weeks of the semester are super hectic and you don't have the time for the elicitation process.

_Major Artifact_: [Requirements Elicitation Document]({{ site.data.externallinks.requirements_report_template }})  , due within the first few weeks of the semester    

__Testing Manager__ - The Testing Manager is responsible for ensuring that the system is thoroughly tested, for developing the overall testing plan/philosophy of the team, and spearheading the beta testing effort at the end of the semester.  The Testing Manager is responsible for executing beta testing at the end of the semester and creating the Beta Testing Document.  The Testing Manager is also responsible for overseeing that philosophy throughout the semester, ensuring unit tests are being written.  Note that the Testing Manager does not write every test case in the system - they just keep up with what everyone else is doing and lend support as needed.

* Reasons to be the Testing Manager: You want to learn more about testing procedures; you love seeing that unit test result bar turn green; you took HCI or something similar and are interested in setting up user testing.
* Reasons not to be the Testing Manager: You don't see the value in writing tests; you don't want to work with your fellow students in doing in-person testing.

_Major Artifact_: [Beta Testing Report]({{ site.data.externallinks.beta_testing_report_template }}), due near the end of the semester    

__DevOps Manager__ - The DevOps Manager is the support tech for the team in a sense.  They are responsbile for the management and support of all the systems we are using in the class, namely GitHub, GitHub Actions, and Heroku.  They should be a person that is relatively comfortable tinkering with computers and settings.  The DevOps Manager does not have to have all the answers, but would be the contact person for going to the staff to get help on any particular issues.

* Reasons to be the DevOps Manager: You are familiar with the tools mentioned already, or you are really interested in learning more about them; you like to tinker with settings to get things working "just right"; you have the patience to help those on your team who might need assistance getting their environments working.
* Reasons not to be the DevOps Manager: You do not feel comfortable helping others with technical issues; you are very unfamiliar with the tools above and would rather just have a "turnkey" solution for doing your work this semester.

_Major Artifact_: [DevOps Report]({{ site.data.externallinks.devops_report_template }}), due near the end of the semester  

__UX Designer__ - The UX (user experience) Designer is responsible for the overall look-and-feel of the project.  They are responsible coming up with the design of the overall app and managing the styling on all pages.  This person would hopefully have the most HTML/CSS/JS experience of the team, but that is not necessarily required.

* Reasons to be the UX Designer: You are familiar with HTML/CSS/JS and/or Bootstrap and you enjoy thinking about how you want people to interact with your application.  You are a person who wants to make sure you turn in a "good looking" app.
* Reasons not to be the UX Designer: You have absolutely no experience with web design and, in fact, you think Geocities pages from the late 90s was the peak of web design.  For some fun examples, see [https://www.cameronsworld.net/](https://www.cameronsworld.net/).

_Major Artifact_: [Usability Assessment]({{ site.data.externallinks.ux_report_template }}), due near the end of the semester  

__Sixth Team Member__ - If your team has 6 members, the member without a role listed above should come to office hours with the professor to discuss options.  The role will be determined based on interest and needs of the team.

## Artifact Document Templates

### Team Documents
{: .no_toc }
[Sprint Report]({{ site.data.externallinks.sprint_report }})    
[Final Submission Pledge]({{ site.data.externallinks.final_submission_pledge }})

### Scrum Master
{: .no_toc }
[Scrum Master Final Report]({{ site.data.externallinks.scrum_master_report_template }})

### Requirements Manager
{: .no_toc }
[Requirements Elicitation Document]({{ site.data.externallinks.requirements_report_template }})      

### Testing Manager
{: .no_toc }
[Beta Testing Report]({{ site.data.externallinks.beta_testing_report_template }})

### DevOps Manager
{: .no_toc }
[DevOps Report]({{ site.data.externallinks.devops_report_template }})

### UX Designer
{: .no_toc }
[Usability Assessment]({{ site.data.externallinks.ux_report_template }})

## Sprint Information

For each sprint check, your team must meet the minimum requirements shown below for each sprint to earn full XP.  Faculty will not override a TA's decision except in extreme circumstances.  

Each sprint is graded out of 25 XP.  In general, the following grading standard applies:

* 25 XP: Excellent progress toward completing the project on time and meeting all requirements.
* 20 XP: Good progress toward completing the project, but at least one requirement looks a bit uncertain.
* 15 XP: Fair progress toward completing the project, but team will need to step up to finish successfully.
* 10 XP: Poor progress toward completing the project and the team definitely needs to refocus.  Some measurable work was accomplished, however.
* 5 XP: Little progress was made toward completing the project during this sprint.
* 0 XP: Project is in danger.

### Sprint 1: {{site.data.semesterinfo.sprint_1.goal}}

__Sprint Duration:__  {{site.data.semesterinfo.sprint_1.duration}}    
__Sprint Due:__ {{site.data.semesterinfo.sprint_1.sprint_check}}

__Goal:__ Have your initial meeting as a team and determine who will be doing what on the team.  This meeting can be any time between when your team is formed and your sprint check meeting with your TA on the first Sunday or Monday of the sprint.  The Scrum Master of each team MUST complete this form with the team as a part of the Sprint: [Team Declaration Form]({{ site.data.externallinks.team_declaration_form }}).  Also, Scrum Masters should initialize the team GitHub repo through [GitHub Classroom]({{ site.data.externallinks.github_classroom_project }}).  Please use your assigned team number for the identifier when prompted (e.g. A-03).  Other team members can then go to that link and accept the assignment, selecting the proper team.

__Requirements:__  Complete the Team Declaration form above ASAP.  Initialize your GitHub repo and have all team members join.

__Team Evals:__ No Team Evals this week.

__How To Submit:__ Scrum Masters should fill out a [Sprint Report]({{ site.data.externallinks.sprint_report }}) and submit it to Gradescope BEFORE meeting with your TA so they can reference it.  Scrum Masters *must* select their team members in Gradescope when submitting so all members will earn the XP for the sprint.  (No, you won't have much to report this week, but think about what's coming up and discuss that.)

### Sprint 2: {{site.data.semesterinfo.sprint_2.goal}}

__Sprint Duration:__  {{site.data.semesterinfo.sprint_2.duration}}    
__Sprint Due:__ {{site.data.semesterinfo.sprint_2.sprint_check}}

__Goal:__ Spend most of this sprint working as a team to elicit the full requirements for your system.  Note that while the final Requirements Document is the responsibility of the Requirements Manager, ALL TEAM MEMBERS are expected to contribute to gathering and refining the final set of requirements.  Once you have a good set of user stories / issues / tasks for your team to work on, add these as Issues to your GitHub Issues page on your team's repository.

__Requirements:__ The team must have a reasonable set of user stories / issues in GitHub Issues.  The Requirements Manager will receive a separate score for the requirements document.

* [Example Requirements Document from Spring 2020](https://docs.google.com/document/d/1l39MWsVEX8LWcQ16Wo5-PXyaKhfm_O6j-1Uj6wj8RUU/edit?usp=sharing)
* ["Excellent" Example from Fall 2020](https://docs.google.com/document/d/1aqeWWhA1QztrM_6iAI1PF3FjP8VTvOqCXhe5w9D9GaU/edit?usp=sharing)
* ["Great" Example from Fall 2020](https://docs.google.com/document/d/12a8MTkqiUZbnDIs-xRfmCQUb8ozs3jHamdcwp6fuqSc/edit?usp=sharing)
* ["Good" Example from Fall 2020](https://docs.google.com/document/d/1RxUBAEFjk0HpQ1aFOOX830nenFBX_Idao3vRVBYop1A/edit?usp=sharing)

__Team Evals:__ At the end of Sprints 2-6 and at the end of the semester, you will need to fill out an evaluation for _each member_ of your team! You can find the evaluation form here: [Student Team Sprint Evaluations]({{ site.data.externallinks.sprint_team_evaluations }})

__How To Submit:__ Scrum Masters should fill out a [Sprint Report]({{ site.data.externallinks.sprint_report }}) and submit it to Gradescope BEFORE meeting with your TA so they can reference it.  Scrum Masters *must* select their team members in Gradescope when submitting so all members will earn the XP for the sprint.  Your GitHub Issues page should be populated with your team's project requirements.  The requirements manager should submit the requirements document to the appropriate assignment.  No other team members should submit the requirements document.

### Sprint 3: {{site.data.semesterinfo.sprint_3.goal}}

__Sprint Duration:__  {{site.data.semesterinfo.sprint_3.duration}}    
__Sprint Due:__ {{site.data.semesterinfo.sprint_3.sprint_check}}

__Goal:__ All projects must have a user account feature for students to login with.  To accomplish this, you are to integrate Google login to your app.

__Requirements:__ A user with a Google Account (not just a Netbadge account!) can login to the system and the system shows in some way that that user has indeed logged in.  You should not lock your app to just @virginia.edu accounts.  You must show that both a regular user account _and_ an admin account can login and that they get different screens.  Print the user's name and account name to the screen to show that it works.  If you want to start working on more requirements, you absolutely can do so.  Your team must be updating GitHub Issues as appropriate throughout the rest of the project.

__Team Evals:__ At the end of Sprints 2-6 and at the end of the semester, you will need to fill out an evaluation for _each member_ of your team! You can find the evaluation form here: [Student Team Sprint Evaluations]({{ site.data.externallinks.sprint_team_evaluations }})

__How To Submit:__ Scrum Masters should fill out a [Sprint Report]({{ site.data.externallinks.sprint_report }}) and submit it to Gradescope BEFORE meeting with your TA so they can reference it.  Scrum Masters *must* select their team members in Gradescope when submitting so all members will earn the XP for the sprint.  The main branch of your GitHub repo should be live on Heroku.

### Sprint 4: {{site.data.semesterinfo.sprint_4.goal}}

__Sprint Duration:__  {{site.data.semesterinfo.sprint_4.duration}}    
__Sprint Due:__ {{site.data.semesterinfo.sprint_4.sprint_check}}

__Goal:__ There are two major milestones for all projects: incorporating the Google Maps API and providing a means for admin users to approve submissions from regular users.  For this sprint, create the infrastructure for doing one of these two things (Sprint 5 will focus on the milestone you don't choose) and implement it in a meaningful way in the system to show significant progress.  The milestone you choose is up to your team, based on the priority of your gathered requirements.

__Requirements:__ In the opinion of the TA, significant work was accomplished this week on one of the two milestones such that it is visible and mostly usable in the system.  GitHub Actions CI MUST be operational with at least multiple test cases in order to earn full XP.  As you are just getting started with testing, this is more showing us that you have the process setup and that you have some passing tests.  Your team must be updating GitHub Issues as appropriate throughout the rest of the project.

__Team Evals:__ At the end of Sprints 2-6 and at the end of the semester, you will need to fill out an evaluation for _each member_ of your team! You can find the evaluation form here: [Student Team Sprint Evaluations]({{ site.data.externallinks.sprint_team_evaluations }})

__How To Submit:__ Scrum Masters should fill out a [Sprint Report]({{ site.data.externallinks.sprint_report }}) and submit it to Gradescope BEFORE meeting with your TA so they can reference it.  Scrum Masters *must* select their team members in Gradescope when submitting so all members will earn the XP for the sprint.  The main branch of your GitHub repo should be live on Heroku.

### Sprint 5: {{site.data.semesterinfo.sprint_5.goal}}

__Sprint Duration:__  {{site.data.semesterinfo.sprint_5.duration}}    
__Sprint Due:__ {{site.data.semesterinfo.sprint_5.sprint_check}}

__Goal:__ There are two major milestones for all projects: incorporating the Google Maps API and providing a means for admin users to approve submissions from regular users.  For this sprint, work on whichever milestone you did not work on for Sprint 4 and implement it in a meaningful way in the system to show significant progress. 

__Requirements:__ In the opinion of the TA, significant work was accomplished this week on the other milestone such that it is visible and mostly usable in the system.  GitHub Actions CI must still be working.  Your team must be updating GitHub Issues as appropriate throughout the rest of the project.

__Team Evals:__ At the end of Sprints 2-6 and at the end of the semester, you will need to fill out an evaluation for _each member_ of your team! You can find the evaluation form here: [Student Team Sprint Evaluations]({{ site.data.externallinks.sprint_team_evaluations }})

__How To Submit:__ Scrum Masters should fill out a [Sprint Report]({{ site.data.externallinks.sprint_report }}) and submit it to Gradescope BEFORE meeting with your TA so they can reference it.  Scrum Masters *must* select their team members in Gradescope when submitting so all members will earn the XP for the sprint.  The main branch of your GitHub repo should be live on Heroku.

### Sprint 6: {{site.data.semesterinfo.sprint_6.goal}}

__Sprint Duration:__  {{site.data.semesterinfo.sprint_6.duration}}     
__Sprint Due:__ {{site.data.semesterinfo.sprint_6.sprint_check}}

__Goal:__ After Sprint 6 is complete, you are going to have other students test your system.  So you need a working system with most all of your functionality ready to go.  The app may not be fully polished and still needs a bit of work, but it needs to be usable from beginning to end.  Your team must be updating GitHub Issues as appropriate throughout the rest of the project.

__Requirments and Full Beta Version:__ In the opinion of the TA, you have an app that is ready for other students to test out (e.g. it doesn't crash, it looks reasonably good, it has most features, etc.).  You will earn 25 XP for the sprint check plus 100 XP as the first half of your overall project score of 250 XP (basically, if you have a working app at this point, we know your final project grade will be at least 100/250 XP, so we can give you those points now).

__Team Evals:__ At the end of Sprints 2-6 and at the end of the semester, you will need to fill out an evaluation for _each member_ of your team! You can find the evaluation form here: [Student Team Sprint Evaluations]({{ site.data.externallinks.sprint_team_evaluations }})

__How To Submit:__ Scrum Masters should fill out a [Sprint Report]({{ site.data.externallinks.sprint_report }}) and submit it to Gradescope BEFORE meeting with your TA so they can reference it.  Scrum Masters *must* select their team members in Gradescope when submitting so all members will earn the XP for the sprint.  The main branch of your GitHub repo should be live on Heroku.

### Beta Testing

__Sprint Duration:__  {{site.data.semesterinfo.beta_testing.duration}}     
__Sprint Due:__ {{site.data.semesterinfo.beta_testing.sprint_check}}

__Goal:__ You now have a "working" version of your project that you can have others use.  Follow the instructions in the Beta Testing Document to have others work through a script of testing your software, similar to what we did with the Guided Practice.  You can ask anyone to test your system, even those currently in CS 3240.  It would be nice to ask at least some folks that you included in your requirements elicitation so they can see what all you have built!  Note that your UX Manager will also need to do the Usability Assessment during this time as well.  Refer to the lectures where this was discussed for more information.  Once you have done your testing, keep polishing your system for final submission!

### Final Version

__Sprint Duration:__  {{site.data.semesterinfo.final_version.duration}}     
__Sprint Due:__ {{site.data.semesterinfo.final_version.sprint_check}}

## Final Grading Information

The final project is worth a total of 250 XP.  (100 XP will be awarded after Sprint 6 for your Beta version and the remaining 150 XP will be awarded by the professors after final demos.)  Like the other assessments in this course, grading is overall wholistic - that is, there is no specific point-for-point breakdown for the rubric.  One reason for this is that this is simply not how software is delivered in real-life.  There are basically only four outcomes:

* You meet the expectations of the customer within reason and both parties are satisfied with the outcome;
* You exceed the expectations of the customer, potentially generating more good will, a good reference, or more future business;
* You do not quite meet the expectations of the customer, leaving some room for improvement;
* You ship a system that simply does not work to the expectations of the customer.

We will grade your projects in a similar vein, with some flexibility for minor adjustments.

Thus, the grading levels will be:

* Above and Beyond - Min XP: 250 / Max XP: 255
* Complete - Min XP: 200 / Max XP: 250
* Lacking - Min XP: 150 / Max XP: 200
* Insufficient - Min XP: 0 / Max XP: 150

Aspects that will determine the exact grade within a range include but are not limited to:

* UI design
* Overall flow of application
* Special features
* Obvious bugs that should have been corrected
* Polish

__Final Team Evals:__ All team members will complete a final, overall team evaluation at the end of the course.  [Final Student Team Sprint Evaluations]({{ site.data.externallinks.final_team_evaluations }})

__Team Project Demo Signup Sheet:__ Do to a number of confounding factors, teams are no longer required to demo their project to earn a grade.  Prof. Sherriff will grade all projects on Monday and Tuesday (Dec 4 & 5) and provide scores ASAP.  Any team that feels that they need to demo their project to Prof. Sherriff due to grading errors can sign up for a time slot the week of Dec 11.  Teams do not need to prepare anything for the demo, but it would be good to make detailed notes about what needs to be discussed.  [Team Project Demo Signup Sheet]({{ site.data.externallinks.final_project_demo_signup }})

__Final Team Project Links:__ Scrum masters should fill out this form after scheduling the demo for the team.  [Project Submission Demo Prep]({{ site.data.externallinks.final_project_heroku_links }})

__The final version of the project must be in GitHub and hosted on Heroku no later than {{ site.data.semesterinfo.project_due_date }}!__