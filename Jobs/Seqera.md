# [Seqera](https://www.seqera.io/careers/senior-software-engineer/)

Also [this more junior role](https://www.seqera.io/careers/backend-software-engineer)

## Prev experience with nextflow
- Built [tmerge analysis pipeline](https://github.com/jacobwindsor/tmerge-analysis-pipeline) using DSL2
	- [tmerge2](https://github.com/jacobwindsor/tmerge)
- Gave presentation to my team on nextflow

## Initial interview with Cyn
[cynthia.benitez@seqera.io](cynthia.benitez@seqera.io)

- Went well
- Said they may be able to find a job specifically for me

## Notes from talks
### Visualiztion of DAG 
- Useful to have a visualization of the process of a pipeline along the DAG
- For tower
- I like these kind of UIs
	- Think of some ideas

## Nextflow schema
- Used to generate a form for a non-dev to fill in parameters to run the pipeline through nextflow tower
- **Have a look at the docs for this**
- How are these forms generated?
	- How is the validation done?
- Very similiar to what we're doing at HCA

### Questions to ask
- What's the architecture of nextflow tower?
	- Agent inside environment running that receives HTTP calls?
	- Obviously many of the features between the CLI and tower are shared, how is code not duplicated?
			- e.g. reading config files, deploying to env
- Comment: datasets and the schema for it is an awesome feature
- Future of tower?
	- Hooks on additions to buckets
	- Event based?
		- Hooks etc?
	- 
- How is nextflow tower supporting SPOT in AWS?
	- spot instances allow using instances that dont have a high availability in their SLA
- Thoughts on fixing the cold start problem of spinnng up instances?



## Behavioural interview with [Matteo Findesio](https://www.linkedin.com/in/mfiandesio/?originalSubdomain=es)
https://devskiller.com/45-behavioral-questions-to-use-during-non-technical-interview-with-developers/

## Projects
- Webpack (**exceeded expectations, self-driven, goal oriented, ownership***)
	- During initial days at abcam
	- Was given free time to explore the codebase since boss was on holiday
	- Problem: Recognised the outdated nature (not using es2015+, build tools, dated tech)
	- Created a branch called "webpackify" and started hacking away
	- Showed boss a small sample and explained why it was a good thing
	- He agreed and we dedicated a couple of months to getting it done
	- Whole team was pleased with the result
	- Allowed us to use modern practices while still supporting older browsers
- Project catalogue (**ownership, leading, deadline, mentoring**)
	- Given the role as tech lead for the project catalogue
	- Collaborated with bioinformatian and given requirements by stakeholders
	- Uncertain if the project would be permanent so built quick MVP
	- Built MVP using tech that would be fast but also easy to convert to something more stable (Angular)
	- Built basic stack with components that would be easy to replace with more stable and maintainable components
	- Successfully completed by the deadline and approve by stakeholders
	- Mentored other new devs to bring them onto the project so it could grow
- GitLab CI/CD (**idea, self-driven, ownership**)
	- Problem: Noticed no automated CI/CD in all of our components at HCA
	- Assessed what was used in other teeams for CI/CD
	- Found out that EBI have there own self-managed GitLab server
	- Drew up a plan and got approval from team lead
	- Converted all of our projects piece-by-piece to have autmated CI/CD
	- Now have *de-facto* ownership of CI/CD and am "go to" guy for any issues
	- Has increased our productivity and dev enjoyment by a large amount (hard to measure)
- Grafana monitoring (**idea, self-driven, ownership**)
	- Problem: hard to track down bugs across our application as no centralised monitoring system and logs lost when deployments happened
	- Assessed current monitoring solutions out there and due to our custom requirements built something
	- Built a monitoring solution with grafana, prometheus, loki, and helm
	- Now "go to" guy for monitoring
	- Still on going project
- Google Summer of COde (Pathway presenter)
	- After very successful bachelor thesis project working with WikiPathways
	- I proposed to continue the project by creating another tool to help visualize metabolic pathways called Pathway Presenter
	- Proposed project to my supervisor, and eventuall GSoC, got approval
	- Achieved the project goals and more 
	- By the end, students in the lab were using it within their presentations
	- Offered PhD
- Optimizing UI build times
	- Noticed early on in my job that we had about 5 minutes downtime on the UI everytime the UI was deployed
	- Noticed, proposed a simple solution, by re-writing environment variables in the post-build artefacts
	- Quick solution, now no dowtime

### Major obstacles
- Direct to CellXGene submission (person & people)
	- Lack of clear requirements and a poor solution proposed by team-mates 
	- Original idea was to base off of a script that was poorly maintained, written, not fit for requirements
	- Recognised that would have to re-write the script and also would most-likely experience blockers from it in the future with bugs due to poor maintainability
	- Drew up a plan with sequence diagrams to build our own solution
	- Didn't immediately get approval because team lead convinced that we could use original script like a "black box"
	- After spending a few hours investigating whether this was possible, I went to him and explained why it would be more difficult and not worth the time
	- Now reached a conclusion to investigate our own way to do this
	- Issues compounded by collaborators in west coast of US
- tmerge - original idea not working
	- Original algorithm of "merging" transcript models was not working as expected
	- Provided lower sensitivity and precision than the original version of tmerge
	- Went to my supervisor, explained the problem to him and 
- Abcam - pushback from colleague on modernistation
	- After seeing the state of front-end code at abcam, I was pushing for modernistation using functional programming practices, modularisation, Webpack, babel, SASS, etc.
	- Approval from boss but pushback from another colleague
	- Wanted to get whole team whole-heartedly on board
	- Prepared presentations and workshop sessions with the team to explain why these are now good practices and create a dialogue to engage my colleague who was pushing back
	- After a few sessions he became convinced that this was a good direction to go
	- However, because I had created a dialogue, I also learnt from him and we reached a conclusion that was mutually beneficial

### Several projects at once
- Often working on several projects at EBI
	- Nature of our work includes a lot of context switching and dealing with emergent bugs
	- Work as a team to prioritize tasks
	- Often talk to colleagues to figure out the best way to solve a problem in the simplest fashion
### Adjusting to changes which weren't expecting
- Covid
	- I am sure everyone experienced these changes during difficult times
	- I was working on my master thesis
	- Was first stuck in Montsant unable to figure out where to go
	- Had to help friends who live in the UK and were stuck in Spain
		- They stayed at my house
	- Had to cope with exams, master thesis deadlines and mental health stress
	- Got computer from CRG
	- Set up regular meetings with my supervisor to maintain some contact without going to the lab
	- Had a delay of 2 months in completing my thesis
	- Achieved the same results I originall wanted despite complications
	- Got job at EBi while working remotely, in unprecedented times
- Stuck in Mexico for two weeks extra due to flights getting cancelled
	- Told boss that it might happen well in advance when I was warned by the airline
	- gave a plan that I would work from 7AM MX time so I would have overlap while still taking care of my mental health and not working completely on UK ime
	- WHen it happened, I found accomadation that had a good coworking space, that I could afford and good internet connectivity
	- Worked productvvely and was commended for efforts during that time
### Communication
#### Miscommunication with supervisor
- Misunderstood a task about exporting projects and what was neededd
- Task was about exporting projects from AWS to GCP and we were experiencing issues with a specific subset of projects
- The user story was not very well written and I had understood it as an optimisation task to improve the speed of exporting
- Made a plan and had begun work on it before hitting issues and asking supervisor for help
- He noticed what I was doing and informed me that it was not neccesary
- Although wasted about 1 day it was good that it was caught early
- We changed the line of work and agreed the plan I had made would be a good thing to do one day
- We also agreed to bring up the user story issue in the retro and the team has now significantly improved at writing user stories

#### Disagreements with colleagues
- **Dylan**
- Our git process
	- disagreed that our git process was fit for purpose - we had uneccesary merges and too many branches
	-  Proposed a solution and received pushback from colleagues that had been using this process for a long time
	- Drew up a document outlining the pros and cons of a few different ideas
	- In the end, got approval but not for what I originall wanted. I created a dialogue and we reached a solution that satisfied everyone and was better than my original idea
#### Not communicated well enough
- Solution for graph validator
	- Was given a project to automate a process
	- Drew up an idea in my head and started working on it
	- Got pushback from colleagues a few days later about my design
	- I hadn't drawn up sequence diagrams or described the flow in detail to my colleagues prior to starting
	- Did do that in the end, and they agreed with me but it was a hurdle that could have been overcome
#### Communicating to non-technical speakers
- BIST poster session
	- Presented a poster of my project to an audience of varying knowledge (most phyicists)
	- Made the poster easy to understand with just flow diagrams and little text
- Gabs
	- Often communicate with gabs the project manager and she is not technical
	- Have become her go to for questions about certain aspects of our system
	- 

#### Depending on others
- Often depend on others
	- Nature of how I work is collaborative and I like to ensure other team members are aware of what I am doing at the very lest

### Small problem detecting
- Submission Envelope flow
	- Noticed this a year ago near when I started. Had many discussions but didnt lead anywhere
	- Now we have a requirement that our current architecture makes it difficult to achieve (although not impossible)
	- Bought it up, got interest of team lead, and his boss as well
		- His boss was the original designer of the system
	- Discussions with Tony about original design choices and why
	- Drew up some vague ideas and hosted a brainstorming/design sessions with new colleagues who are not entrapped in the current way of thinking
	- 
