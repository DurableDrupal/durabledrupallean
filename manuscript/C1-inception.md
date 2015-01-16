# Chapter 1. Project Inception {#chapter-01}

We are diving right into a real world project, the Durable Drupal Website, in order to demonstrate. But just where do we dive in? Where does inception live?

## First team meeting.

We start with an empty Kanban board. There are four columns:

* New
* To do
* In Progress
* MVP 1

Jeff is using [Trello](https://trello.com/) to create the board (Figure 1-1).

![Figure 1-1. Empty Kanban Board for New Project](images/c1_01.jpg)

I> Why Kanban? And what is Kanban, exactly? Well, the original [Kanban is a lean manufacturing process](http://en.wikipedia.org/wiki/Kanban). It comes from the world of the nuts and bolts production chain, and is a system of logistical control. "Kanban was developed by [Taiichi Ohno](http://en.wikipedia.org/wiki/Taiichi_Ohno), at Toyota, as a system to improve and maintain a high level of production. Kanban is one method to achieve JIT". (JIT is the [Just in Time](http://en.wikipedia.org/wiki/Just_in_time_(business)) production strategy). 
I>
I> Now, just as this production strategy was put into place with great discipline and sacrifice by Toyota and other companies in order to survive the booms and bubbles as well as the bursts ([Lost Decade](http://en.wikipedia.org/wiki/Lost_Decade_(Japan))) inherent in the world capitalist economy, [Kanban for software developers](http://en.wikipedia.org/wiki/Kanban_(development)) (and all [knowledge workers](http://en.wikipedia.org/wiki/Knowledge_workers)) is a wonderful way to optimize energies and resources of all kinds through a just in time delivery flow in our own neck of the woods.
I> Above and beyond Drupal or any other framework or stack we might be using, one of the principal objectives of this book is to show how we can move from Kanban, Agile and Lean as buzzwords to success through actual best practices

A team meeting is held to get the ball rolling. The team is made up as follows:

* Anna (Product Owner)
* Jake (DevOps)
* Mark (UX)
* Jeff (Back end)
* Lisa (Front end)
* Victor (Project Coach)
* Sherrie (Graphic design)

Anna starts the meeting by reading out a vision of what a minimum viable product ([MVP](http://en.wikipedia.org/wiki/Minimum_viable_product)) might be in this particular case:

> We can share a solution we have found: to calmly concentrate on the real needs of the users (biz needs of user as solution provider and user needs of that biz's users) and become their [advocate](http://alistapart.com/article/from-empathy-to-advocacy). Never mind the desperate mystification of the rock stars and the gurus, the smoke and mirrors and the [fear, uncertainty and doubt (FUD)](http://en.wikipedia.org/wiki/Fear,_uncertainty_and_doubt) they disseminate. Cutting to the [Core](http://alistapart.com/article/the-core-model-designing-inside-out-for-better-results) with our approach can help any team willing to commit themselves to a disciplined approach systematically tool up to determine step by step what is needed and how to get there using readily available tools and methods.
> 
> By using a solid Drupal distribution that has a best and rich set of modules for most use cases that you can just download and use (among others tailored for other use cases), which can then be curated to evolve with the special needs of the workshop, and by adopting a lean process tailored to that framework, folks can avoid the confusion, smoke and mirrors and false pitfalls that emerge only due to a lack of information, confidence and method.

> We can offer that in a series of books and media packages now and into the future, whatever it may behold in terms of operating systems, stacks and frameworks, to show how all of this can evolve and migrate in any workshop willing to apply serious workmanship for the long haul. We can offer a journey into the future by accompanying migrations into Backdrop, Drupal 8 and other frameworks and full stack development, showing how to migrate over time existing drupal websites and web apps to those frameworks and environments.  

> We can help many small and medium website and web app development workshops survive and thrive.

At this point Victor proposes that the team build a prototype in order to prepare for the [Project Kickoff](#chapter-02). At the Kickoff the team will cut to the core of that vision, revealing what the project is really about and reaching team consensus on the what characteristics the initial value testable MVP will have and what jobs of work need prioritizing in order to make that delivery.

The prototype needed as prep for the kickoff can be as simple as a home page featuring a suitable version of the project vision and an email signup form. This provides a snap starting point on an immediate concrete footing. The build process will have a lot in common with upcoming MVP iterations, allowing for initial decisions to be made on tools, stacks, frameworks and infrastructure. 

The meeting is now used to plan out on the Kanban board the actual jobs of work needed so that the team can build the prototype as quickly and directly as possible. 

After some discussion, the Kanban board looks like this:

<< image >>

The main thing to understand about Kanban is that it is not based on the pre-estimated "sprints" designed to deliver a complete mini-release one finds when using Scrum. Rather it is a continuous flow process. Core outcomes are implemented one at a time, and their associated issues pass through various states (represented by columns) in the process. At the start all issues are placed in the New column (state). Then a few are prioritized and are placed in the limited backlog "To Do" column, which is a limited column. When team members work on an issue, it is placed in the "In Progress" or "Doing" column. This column is also limited in the number of issues it can contain. The reason for this is the key to why Kanban is different: it champions focus and prohibits people working on too many things at the same time. This is called a Work in Progress (WIP) limit, and it replaces the constraint of the sprint cycle length found in Scrum. In this way, Kanban frees us from waterfall-like mini-release "estimates". So while there are no sprints, only a continuous flow of jobs of work being delivered for value testing, the key constraint for each state is to be found in the WIP limit, seen in parenthesis in the To Do and In Progress column titles. The actual number is calculated and optimized by taking into account team size and velocity, and is adjusted for maximum productivity without overloading the team as the project matures.

Another benefit is that since the focus is on jobs of work and not abstract mini-releases, it is much easier to foster multi-discipline cross-collaboration. 

Lets take a look at the individual (tasks, wot?)

vision -> cut to the core in kick-off meeting
provisioning of team dev environments 

First of all, everything is pushed into the New column. Then ...

We limit the To Do column and the Doing column to 3 (number of separate disciplines being worked on with semi-paired programming).

There were a couple of heated discussions.

## frameworks to be used

## provisioning for dev environments

## deployment

## other tasks needed to plan for the kick-off