# Appendix 1. DurableDrupal Lean Process. Overview {#appendix01}

What follows is an overview of how to make use of the process. There are also links drilling down to templates you can use immediately as your project gets going. 

T> If you would like more background as to why Agile and why Lean, please feel free to skip first to the [Agile Software Development. Background and Resources](#agile-background-resources) section.
T>
T> We will describe the process via a listing of typical chronological steps and activities, although it is important to bear in mind that certain projects will want to tailor the use of the tools and artifacts in accordance with their own specific characteristics. 


TODO place this snippet somewher: For example, just in order to complete the initial MVP vision, some projects will warrant a fully-functional MVP prototype or test landing page before going any further, while others will base their first prototype on a set of user stories.

## Project inception {#appendix01-project-inception}

### Initial contact with the project owner 
Somewhere, somehow the project is born. A telephone call or an email is received, a comment made during a chance encounter on the street or at the mall. The job of the agency member is to initiate an organized process involving a job of work. As such, an invitation is issued for a meeting, either in person or through a remote service such as [Skype](http://www.skype.com/en/) or [Google Hangouts](https://plus.google.com/hangouts). Once the invitation is accepted, the project is born.

At this point, an agency member opens up a [Kanban board](http://en.wikipedia.org/wiki/Kanban_board) for the project. DurableDrupal Lean works very well with the light-weight and powerful [Trello](https://trello.com/), but you can use any other alternative you are familiar with, including the following (most have some kind of free account):

* Build your own
  * [Make a personal Kanban board](http://www.instructables.com/id/Kanban-Organization-thru-post-it-notes/)
  * You can use a whiteboard with post-it notes and then take photos to capture state
  * [Kanban examples](http://leankit.com/kanban/kanban-examples/)
* [Mingle](http://www.thoughtworks.com/products/mingle-agile-project-management)
* [Pivotal Tracker](http://www.pivotaltracker.com/)
* [Fulcrum](https://github.com/fulcrum-agile/fulcrum) Open source clone of Pivotal Tracker
* [Gitban](http://www.gitban.com/) Worth trying since it uses Github Issues directly from your repo
* [HuBoard](https://huboard.com) Another Kanban board built on top of Github Issues
* [LeanKit](http://leankit.com/)

After creating a new board, generally three columns are created:

 



Whether it's during a meeting with a prospective client or an interview after having submitted an RFP (Request for Proposal), a dialog is started concerning the building of a product capable of solving a specific problem felt by a significant group of people.






Laura Klein, author of [Lean UX - Applying Lean principles to Improve User Experience by Jeff Gothelf and Josh Seiden](http://www.jeffgothelf.com/blog/lean-ux-book/#sthash.22gOyp12.dpbs) ... m p p

Q> ### Defining Market, Problem and Product
Q> "A market is the group of people you think might want to buy your product.... A problem is the reason that those people are going to use your product... A product is simply the way that you’re going to solve the user’s problem. It’s the end result of what you’re building. It’s the thing that people, presumably in the target market, are going to pay you money for." (Klein, Chapter 1)
Q>
Q> ### On Validating the Problem
Q> "You are going to discover a problem that exists within your target market that you are capable of solving. Remember, if there’s no problem, then there is no compelling reason for people to purchase your product.... You’ll know that you’ve validated a problem when you start to hear particular groups of people complaining about something specific."
Q>
Q> ### On Validating the Market
Q> "Validating the Market: You’ll know that you’ve successfully validated your market when you can accurately predict that a particular type of person will have a specific problem and that the problem will be severe enough that that person is interested in purchasing a solution."
Q>
Q> ### On Validating the Product
Q> "Just because you have discovered a real problem and have a group of people willing to pay you to solve their problem, that doesn’t necessarily mean that your product is the right solution.... You’ll know that you’ve validated your product when a large percentage of your target market offers to pay you money to solve their problem."

So it's important to bring up the method of Validation Driven Design right from the start with the client, and even in the first interviews, learn as much as is possible without further testing and research about the Problem and Market the proposed Product is related to. And to emphasize how all the development, even (especially) after delivery will be concerned with validating all three cornerstones.

The DurableDrupal Lean process helps that along by providing an optional MVP Template. There is a guide on how to work with it. It's optional because we never want to impose an obligatory paper-heavy process on anyone. If you feel this template (and [the other two or three]() we include) helps to organize, so much the better. Feel free.


## Agile Software Development. Background and Resources {#agile-background-resources}

### Introduction

The difficulty of getting a birds' eye view of any software development process is that it is at its heart a grammar and specialized vocabulary, a set of conventions, tools and structures used dynamically and creatively in real world contexts. When it is used of course, it appears as a logical sequence. Like title, author, sections, sentences, phrases, words and expressions in a blog entry, or a series of instructions in a manual. But any attempt at explaining the grammar runs the risk of reducing the whole dialog to boring and lifeless abstractions. 

When we're learning, of course, we need a list of conventions, a vocabulary, and a grammar allowing us to see the options we have in making use of process, and in order to understand the language when we are new to a team.

Remarkably, incremental and iterative software development is nothing new at all, and [goes at least as far back as the Waterfall model](http://en.wikipedia.org/wiki/Agile_software_development#History). 

### Why use process at all

Work is a social process, ever since we gained an opposable thumb. It's also an historical process. Why do we want to engineer things using today's tools and processes? Simply in order to avoid making the same expensive mistakes over and over again, and to avoid inventing the wheel when we tool up for a product.

### Waterfall

The baseline in software development is what is called the [Waterfall Model](http://en.wikipedia.org/wiki/Waterfall_model).

[Winston W. Royce's original article Managing the Development of Large Software Systems](http://www.cs.umd.edu/class/spring2003/cmsc838p/Process/waterfall.pdf) (interesting that even it includes quite a bit on iteration)

A> The waterfall model is a sequential design process, used in software development processes, in which progress is seen as flowing steadily downwards (like a waterfall) through the phases of Conception, Initiation, Analysis, Design, Construction, Testing, Production/Implementation and Maintenance.
A>
A> The waterfall development model originates in the manufacturing and construction industries; highly structured physical environments in which after-the-fact changes are prohibitively costly, if not impossible. Since no formal software development methodologies existed at the time, this hardware-oriented model was simply adapted for software development.[1]
A>
A> > [Wikipedia: Waterfall Model](http://en.wikipedia.org/wiki/Waterfall_model)

In following the Waterfall Model, the various disciplines are executed in a single, non-iterative cycle: Requirements, Design, Construction, Integration, Testing, Installation and Maintenance. 

Waterfall may still be the mest process model for your project if it is static in requirements and it is unlikely or prohibitively expensive for changes to be made and there is an insurmountable need for pinpoint estimates in scheduling and resources.

For many other kinds of projects, however, including most website and web app projects, Waterfall can be a recipe for disaster.

### What's wrong with Waterfall?

In projects where changes are very likely to occur along the way, or in which technology is changing rapidly, the Waterfall Model accentuates the risk of failure:

* Because of the long delay between initial assumptions and requirements gathering and delivery, the probability of erroneous feature sets being implemented that do not really comply with real user and organizational requirements is greatly amplified.
* Because changes (scope creep) are bound to happen (40% of the requirements is a common minimum figure) but are not recognized officially, either the real costs exceed budgeted costs by far, or else long and even critical delays are often occasioned.
* Since testing is not done on the unit, integration and quality assurance levels, the cost and impact of repairing anomalies is much higher and the overall quality of the product suffers.
* Elevated cost of failure means there is no room for error, and leads to a costly fear of experimentation on all fronts.

### Better ways of developing software. The Agile Manifesto

The [Agile Manifesto](http://agilemanifesto.org/), defending a leaner, iterative and incremental approach to software development, bases itself on following 12 principles 

> Our highest priority is to satisfy the customer
through early and continuous delivery
of valuable software.

> Welcome changing requirements, even late in 
development. Agile processes harness change for 
the customer's competitive advantage.

> Deliver working software frequently, from a 
couple of weeks to a couple of months, with a 
preference to the shorter timescale.

> Business people and developers must work 
together daily throughout the project.

> Build projects around motivated individuals. 
Give them the environment and support they need, 
and trust them to get the job done.

> The most efficient and effective method of 
conveying information to and within a development 
team is face-to-face conversation.

> Working software is the primary measure of progress.

> Agile processes promote sustainable development. 
The sponsors, developers, and users should be able 
to maintain a constant pace indefinitely.

> Continuous attention to technical excellence 
and good design enhances agility.

> Simplicity--the art of maximizing the amount 
of work not done--is essential.

> The best architectures, requirements, and designs 
emerge from self-organizing teams.

> At regular intervals, the team reflects on how 
to become more effective, then tunes and adjusts 
its behavior accordingly.

Q> ## This author is proud to have [signed the Agile Manifesto in August 2006](http://agilemanifesto.org/sign/display.cgi?ms=000000067)
Q>
Q> Victor Kane: (AWebFactory) Building software must be built around real human needs, and neither the product nor the process shoved down people's throats. The need for software and the need to produce that software must be framed in a process (the process mirrored in the product - Hudson), is optimized by open, flowing structures reflecting those very real needs and their most excellent solutions. Obstacles imposed by greed and the need to defend privilege must be removed. Working people who produce and use software must together manage that process themselves, worldwide.

### Scrum

TODO Scrum section

### Kanban

TODO Kanban section

Kanban is where Agile and one of its industrial manufacturing predecessars, JIT (Just in Time). And is what gives origin to the today's everyday agile expression "Just enough, just in time".

### Agile and Lean Bibliography

#### Websites

* [The Agile Manifesto](http://agilemanifesto.org)
* [Extreme Programming: A gentle introduction](http://www.extremeprogramming.org/)
* [Agile Software Development: A gentle introduction](http://www.agile-process.org/)
* [Mike Cohn's Scrum and Agile site](http://www.mountaingoatsoftware.com/)
* [Agile @ Adobe Agile Resources](http://blogs.adobe.com/agile/2014/12/05/agile-resources/). Excellent comprehensive list of all kinds of Agile and Scrum Resources

#### Books

* [Extreme Programming Explained: Embrace Change by Ken Beck](http://www.amazon.com/Extreme-Programming-Explained-Embrace-Change/dp/0321278658/ref=sr_1_1)
* [Agile Software Development with Scrum by Ken Schwaber & Mike Beedle](http://www.amazon.com/dp/0130676349). Original Scrum book.
* [User Stories Applied by Mike Cohn](http://www.amazon.com/User-Stories-Applied-Software-Development/dp/0321205685)
* [Kanban and Scrum by Henrik Kniberg and Mattias Skarin](http://www.infoq.com/minibooks/kanban-scrum-minibook)
* [The Lean Startup by Eric Ries](http://theleanstartup.com/book)
* [Lean UX - Applying Lean principles to Improve User Experience by Jeff Gothelf and Josh Seiden](http://www.jeffgothelf.com/blog/lean-ux-book/#sthash.22gOyp12.dpbs)
* [UX for Lean Startups: Faster, Smarter User Experience Research and Design by Laura Klein](http://www.amazon.com/UX-Lean-Startups-Experience-Research/dp/1449334911)
