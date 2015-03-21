# Chapter 3. DevOps. Team Provisioning, Workflow and Configuration Management {#chapter-03} 

## Development Workflow and Everything in (Versioned) Code 

By the time the user stories are written for the current backlog, the whole team has been "kicked off" on each of them. A short excerpt from Gothelf shows what collective development is like as the team works to complete the backlog:

> It’s Tuesday and Rick, Mark, Olga, and Arti are standing at the whiteboard , looking at a wireframe that they’ve drawn. Arti has a marker in her hand, but she’s not drawing. “Rick, I don’t understand what you’re driving at. Can you explain the problem?” Rick takes the marker, wipes clear a section of the board, and explains the regulation again. The team is designing an app for stock traders, and the app has to obey a strict set of regulations. Rick, the business analyst, is responsible for making sure that the team’s designs support the rules. After a while, the team is nodding, and Arti takes the marker again. She suggests a change to the wireframe design of the app on the board and the team nods again. They all take out their iPhones, take photos of the board, and agree to reconvene the next day. They’re confident that what they’ve agreed on will be ready for user testing on Thursday. Arti, the designer, goes back to her desk to start detailing the design they’ve sketched. Mark, the front-end developer, starts building the page — he uses premade components from the living style guide the team has put in place, so he doesn’t need to wait for Arti before getting the basic pieces in place. Rick opens the project’s wiki and begins to document the decisions the team has made about the application behavior. He’ll review these choices with the product owner later in the day. And Olga, the QA tester, begins the process of writing tests for the new section of the app. (*Gothelf, Jeff (2013-02-22). Lean UX: Applying Lean Principles to Improve User Experience*)

"This is the day-to-day rhythm of Lean UX: a team working collaboratively, iteratively, and in parallel, with few handoffs, minimal deliverables, and a focus on working software and market feedback."

### Provision for each Team Member

With the process flowing smoothly, there's nothing to stop us in our Development Workflow. Let's drill down to how this actually works. 

Every team member will need at least:

* Their own working environment as close to target production characteristics as possible
* Gitflow (distributed version control branching model) for all!
* Continuous integration (automated and managed commits, testing and deploy to the integration dev server instance)
* Special workflow for framework idiosyncracies: for example, an "everything in code" strategy for Drupal Development, a SASS environment for Drupal and/or full-stack theming.

Let's examine three possible solutions, at least:

* Rolling our own (the idea was to keep it simple...)
* Kalabox 2 dev environment and tools with, say, Pantheon
* Platform.sh cloud plus local continuous integration environment

### User story: Card, Conversation, Confirmation

The user story template constitutes the Card aspect of the user story and becomes part of the prioritized backlog, as we have seen, during the iteration planning meeting. Once it is actually being worked on, Conversation will take place, and may or may not be captured in the issue tracking system being used. Confirmation refers to user story testing. This includes unit and integration testing on the code, functional acceptance testing by the product owner, as well as market performance outcome testing of the hypothesis or sub-hypothesis. It will only be when the hypothesis is validated by the user and by measurable market outcomes that the card may be moved to the Done column.

### Everything in Code with features demo

A team cannot effectively do Drupal CMS development without using the Everything in Code paradigm.

Drupal by default keeps all its configuration setup interactively in the admin pages as persisted values in the same database where the content is stored. In order to work as a team in development, that is, in order to commit modifications or work completed asynchronously without destroying work commited by others, or content entered by content editors, it is necessary to use a distributed version control repository, as demanded by software development best practices.

Example workflow:

~~Video: The demo starts at minute 14:35 of the demo video (no good in Spanish!)~~

* We change the default theme and change the Site Name
* We create a feature
* We specify elements to include
* We create the feature and save it to the file system
* We enable the feature, moving the configuration of the selected elements to code
* We change the theme and the site name
* We see the feature is overriden (database is overriding code because of the changes)
* We "revert" the feature (force the database to adapt to the code)

