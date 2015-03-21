# Chapter 2. Team Project Kickoff {#chapter-02}

![Gothelf Lean + Scrum](images/gothelf-lean-plus-scrum.jpg)

* Every sprint has a kickoff, not just the first
* Everyone participates
* Domain experts are invited where needed
* May last a few hours or a week, whatever it takes

## What goes on at the Kickoff

The Kickoff is not the planning meeting, which immediately follows it. It creates the raw material and conditions required by the planning meeting, so that there will be something to plan. It consists of brainstorming and validation exercises which will enable the team to define a minimum viable product (MVP) as a set of hypotheses based on the clarification of project problem statements and their underlying assumptions. It's about validating that there exists a Problem that really affects a segment of the Market to the extent they are willing to pay for a Product that effectively solves it:

> We are radically shifting " the way we frame our work. Our goal is not to create a deliverable, it’s to change something in the world — to create an outcome. We start with assumptions instead of requirements. We create and test hypotheses. We measure to see whether we’ve achieved our desired outcomes." 

Let's drill down into the Kickoff process and see how everything fits together and actually prepares for the planning session, where the user stories capable of implementing our Features will find expression.

## Problems, Assumptions, Hypotheses

* We want to clarify the problem statement that has given rise to the project in the first place as much as possible
* We want to list the general assumptions underlying the problem statement at the core
* We then want to prioritize those assumptions in order of risk. The riskiest assumptions will need to be validated first.
* We will want to transform each assumption statement into a hypothesis statement. There are three elements to each hypothesis statement: Features, Personas, Outcomes
  * We list all hoped for Outcomes
  * We detail Personas as we see how Problem, Market and Product relate to each other in our particular case
  * We itemize Features. A team brainstorming mini-session is often used for this. Which features will drive customer behavior towards the outcomes being sought? Features will form the basis for future "themes" around which to unify the team in the course of variously scoped sequences of related sprints. This is a major factor for guaranteeing cross-collaboration. 
  * Once we have Features, Personas and Outcomes we are ready to fill out an hypotheses creation table, each row having the form "We will create <this Feature> for <this Persona> in order to achieve <this Outcome>.
  
At this point we can validate the Outcomes and the Personas by "getting out of the building" and doing research at this point. Of course, we'll have to wait for the implementation of the MVP in order to validate the product and the hypotheses.

Optional tools that can help us achieve all this are: the Problem Statement Template, the Business and User Assumptions Worksheet, the Personas template, the Hypotheses Creation Table, and finally the Hypothesis and sub-hypotheses templates. They are included below in the following sections.

T> Remember, these are not hoops you are forced to jump through. They are proven methods for arriving at our goal of problem and market validation and preparation for the theme or sprint planning meeting. Use whatever actually helps in a given project. Check out the examples in this book and the associated workbooks.

## Problem Statement Template

[Our service/ product] was designed to achieve [these goals]. We have observed that the product/ service isn’t meeting [these goals], which is causing [this adverse effect] to our business. How might we improve [service/ product] so that our customers are more successful based on [these measurable criteria]?


## Problem Statement Example

Our service offers a conduit between job seekers and employers trying to hire them. Through our service, employers can reach out to job seekers in our ecosystem with employment opportunities. We have observed that one critical factor affecting customer satisfaction is how frequently job seekers respond to employer messages. Currently, job seekers are replying to these communications at a very low rate. How might we improve the efficacy of our communication products, thus making employers more successful in their jobs and job seekers more satisfied with our service?


## Hypothesis template

We believe [this statement is true]. We will know we’re [right/ wrong] when we see the following feedback from the market: [qualitative feedback] and/ or [quantitative feedback] and/ or [key performance indicator change].


## Hypothesis example

We believe that creating an efficient communication system within TheLadders’ product experience for recruiters and employers will achieve a higher rate of contact success and an increase in product satisfaction. We will know this is true when we see an increase in the number of replies from job seekers to recruiter contacts and an increase in the number of messages initiated by recruiters in our system.


## Sub-hypothesis template

In most projects we will find ourselves breaking hypotheses down into prioritized lists of sub-hypotheses in order to be able to validate some of the more detailed product features:

We believe that [doing this/ building this feature/ creating this experience] for [these people/ personas] will achieve [this outcome]. We will know this is true when we see [this market feedback, quantitative measure, or qualitative insight].

The prioritized lists of sub-hypotheses consitutes one of the most important results of the kickoff and greatly facilitate planning meetings and user story backlog creation.

## Personas

Instead of having lengthy and costly research serve us up a list of personas never to be questioned, we whip up Proto-Personas on the basis of our Assumptions, then validate and refine them. A letter-sized sheet of paper folded into four squares, with points 1 and 2 across the top, and with 3 and 4 across the bottom is often used:

 1. Atavar or sketch, name, age, city, occupation, etc.
 1. Behavorial demographic information: Marital status, Number of children, their ages, Working conditions, Leisure time, lifestyle, etc.
 1. Pain points and needs
 1. Potential solutions
 
We create Proto-personas, and interview them in the field to validate and develop further. To do this research we need to "get out of the building" ([Steve Blank](http://steveblank.com/2010/03/11/teaching-entrepreneurship-%E2%80%93-by-getting-out-of-the-building/)) to test the problem statement, associated assumptions and derived Proto-Personas. Now, why should a web application development team take advice from an entreupeneur coach?

**Because every project is a start-up!**

## Feature brainstorming

Once we have personas with real problems that have been (ideally) researched and validated, we can brainstorm on features that will drive customer behavior towards the desired outcomes. We brainstorm and  create a list (stick them all up on the wall and then prioritize them).

**Features will be the basis for themes** (focused sets of sprints or work in progress on the basis of plenty of time for designer creativity and cross-collaboration).

## Collaborative Design and Prototype towards Initial MVP

Once we have features, we can work on design!

### Why and what

* Everybody gets to design together
* Low fidelity sketches and artifacts increase collaboration
* Methods such as group design studio build a shared understanding of features across the team

### Methods and techniques

* Collective design studio
* Style guides and pattern libraries
* Special techniques for remote distributed teams

A big proponent of style guides in the Drupal Community, including setting up automated style guides, is [John Albin](https://www.drupal.org/u/johnalbin). See for example [Style Guide Driven Development](https://melbourne2015.drupal.org.au/session/style-guide-driven-development):

> "We suck at what we do. We know the websites we build need excellent front-end performance, full accessibility, compelling designs, and reusable parts. We learn. We plan. We build. We make a mad scramble to finish on time and deliver a product that falls short of what we know we could have achieved. Every. Single. Time."
>
> "And it turns out integrating agile development with web development is actually very simple. It's called *style-guide-driven development*." 

## Iteration Planning Meeting

The classic meeting using everything we've gathered together so far to write user stories (together) and specify the iteration backlog.

Different teams working on different projects may be using Scrum or Kanban approaches. The former will plan by prioritizing a list of user stories to form the sprint backlog, and estimation may be included. With Kanban, velocity will be optimized by applying restrictions on the number of prioritized backlog stories to be included at any one time in the work in progress.

## User story template

Influenced by [A framework for modern User Stories by @jonatisokon](https://medium.com/@jonatisokon/a-framework-for-user-stories-bc3dc323eca9).

**Classic format**

As a [persona, user] I want to [perform action] so that [achievable goal].

**User validation test addendum**

Given that I'm [performing action] ... 
When [point of observation]
Then [observable result]

## User story examples

As a writer I want to save my story so that it can be critiqued.

Given that I have saved my story
When I tap the save icon to save my story
Then saved to my stories and visible to fellow workshop members
