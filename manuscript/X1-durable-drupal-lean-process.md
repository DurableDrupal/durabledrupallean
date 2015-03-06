#  1. DurableDrupal Lean Process. Overview {#appendix01}

DurableDrupal Lean is a process factory, providing reusable tools and methods for a team or team of teams within an organization, with the firm purpose of defeating waterfall and guaranteeing delivered value. 

Now, that's a mighty set of phrases right there. If we understood that sentence and knew how to use it on a daily basis, we could end this right now and go have a beer. Well, let's read on. And then go have a beer. For now, let's hunker down and do what we always do when we want to learn something: deconstruct it, that is, take it apart; and then synthesize our own process by putting it back together again, both abstractly, and then as we work through this book, in actual practice.

* A process factory
  * Because we don't want to take a rigid scheme and mechanically force ourselves to go through motions that may or may not have anything to do with who we are or what we are trying to accomplish. We want to learn how to create, recreate, evolve and maintain our own process, on every team in our organization, for every different kind of project.
* DurableDrupal Lean
  * We must be in the habit of using upstream Drupal distributions in our organization. In this book we are providing one, [DurableDistro](https://github.com/DurableDrupal/durable-drupal-distro), along with an Ansible playbook to easily provision it with Vagrant. W think it will give you a great head start and it can be easily curated as needed; and we also list [a lot of the most useful ones out there](#appendix-02-distributions) which you can use for many specialized purposes right off the shelf. The question as always is to stand on the shoulders of giants.
  * Lean: Agile is the new Waterfall. We need Lean, and we want you to know what this software development process is all about and why it should be important to you.
  * See below for explanation of what is Waterfall, Agile, Lean, etc.
* Reusable tools and methods
  * We want to review them here. Later on you will make your own. We want to keep it down to a dull roar though, in order to avoid top heavy, documentation laden wastes of time.
* For a team or team of teams.
  * We are talking continuous improvement in your organization, whether it's a one man shop (still a team!), an agency or company department with a single team, or a team of teams (we never want to work on a scale bigger than a team when we focus on work in progress). We are talking everyone face to face in a single building, or a world-wide distributed team or team of teams. 
* Guaranteeing delivered value
  * Because code can no longer be implemented on the basis of "functional requirements". Code's sole purpose in living is to be able to test a hypothesis envisioning value to be obtained by the client as a result of its existence. Code should be designed as such, and tested as such. Becuase neither is it enough to test code and be satisfied that it works as advertised in order to consider a job of work completed. The functionality designed to give value must be tested to make sure it actually delivers that expected value to the client. This is at the core of Lean and we'll be sure to drill down here.

In order to gain this insight, as we work through this book we will be needing to get comfortable (not necessarily all at once! we recommend just in time reading as needed, perhaps on a chapter by chapter basis) with the following:

* [A very short history of modern software development process](#appendix01-short-history)
* [Kanban (not Scrum)](appendix01-kanban)
* [Project Inception and Vision](appendix01-inception)
* [Team Kickoff](appendix01-team-kickoff)
* [Development Workflow with Everything in Code](#appendix01-dev-workflow)
* [DevOps, Server Provisioning and Deployment](#appendix01-devops-ci)
* [User Validation](#appendix01-user-validation)
* [Bibliography and Resources](#appendix01-bibliography)

## A very short history of modern software development process {#appendix01-short-history}

Why use process at all? Well, work is social in nature, ever since we humans gained an opposable thumb. And it always exists in an historical context. So we engineer things using today's tools and processes in order to avoid making the same expensive mistakes over and over again, and in order to avoid inventing the wheel every time we tool up for a product.

We need process to avoid wasting time, money and resources. To avoid failing. Again and again.

### The limitations of Waterfall and Agile for Web development

The much criticized [Waterfall Model](http://en.wikipedia.org/wiki/Waterfall_model) is a sequential process for software development "in which in which progress is seen as flowing steadily downwards (like a waterfall) through the phases of Conception, Initiation, Analysis, Design, Construction, Testing, Production/Implementation and Maintenance." Which is to say, outputs are handed off in sequence from one discipline "silo" to another. It is no accident that this method, which at least raised software development from the level of artesanal improvisation to that of engineering, had its origins in the highly structured manufacturing and construction industries.

[Agile software development methodologies](http://en.wikipedia.org/wiki/Agile_software_development) favor an iterative and incremental approach due to the following shortcomings of the Waterfall Model:

* A minimum of 40% in change requests during project lifetime make it impossible for each discipline to  complete its work and then hand-off a perfect output to the next discipline in line since disciplines already "finished" will have to be revisited (i.e. design and even the candidate architecture may have to be re-done in line with the change requests).
* Clients require working prototypes at various stages in order to properly finalize their requirements, so that Construction cannot be carried out in one fell swoop without a series of programmed opportunities for user feedback.
* Design may dictate solutions impossible or very difficult to implement, which can only be seen during the Construction phase. In other words, a lot of design and construction work may have to be thrown away and started over.
* By the same token, design may be dictated by stakeholders who are unaware of the full benefits of the technology, and only become aware as Construction progresses, which is one of the principle sources for the high rate of change requests in most projects.

Diserée Sy's article [Adapting Usability Investigations for Agile User-centered Design](http://uxpajournal.org/wp-content/uploads/pdf/agile-ucd.pdf), published in 2007, first introduces the characteristics of both the Waterfall and Agile software development methodologies, contrasts the benefits of Agile to the deficiencies of Waterfall, and then goes on to enumerate certain "adaptations to the timing, granularity, and reporting used for Agile interactive usability investigations, with an intended audience of usability practitioners."

In other words, Waterfall leads to the creation of isolated discipline silos where deliverables are implemented and then handed off to others without there being anywhere near enough cross-collaboration or feedback. Agile is an improvement over Waterfall since the abyss separating requirements gathering from testing is shorter and since the mini-cycles lend themselves to more testing and feedback taking place. This can be seen in the following diagram from the article:

<< waterfall and agile diagram >>

The problem raised for the work of the User Experience Team and Graphic design in general, is that with Agile the cycles gave ... little ... time

### Improving Agile with Cycle 0 and Staggered Sprints

The solution was to bifurcate UX and Development so that a Cycle 0 (req gather initial meeting) and staggered sprints gave better timing ... so the user experience team could work iteratively and incrementally also. The following diagram from the article shows this:

<< cycle 0 and staggered sprints diagram >>

### Achieving a still better process with Lean UX and Design + Dev



### The Best Process we Know: Design + Dev + DevOps

### Waste that is eliminated by using DurableDrupal Lean

Waste is of course, the opposite of value. We sum up by reviewing the possible causes of waste in software development:

* Unfinished work left rotting in isolated silos
* Feature creep without validating for impact or value
* Isolated silos keep on re-inventing the wheel
* Handoffs chronically disrupts workflow
* Delays because isolated silos and teams missing skills
* Task switching because work overload and broken workflow
* Mucho defect because chaotic focus and blocked knowledge sharing

See also [How to Manage the "7 Wastes" of Agile Software Development](https://www.scrumalliance.org/community/articles/2013/september/how-to-manage-the-7-wastes%E2%80%9D-of-agile-software-deve).

## Kanban (not Scrum) {#appendix01-kanban}


## Project Inception and Vision {#appendix01-inception}


## Team Kickoff {#appendix01-team-kickoff}


## Development Workflow and Everything in (Versioned) Code {#appendix01-dev-workflow}


## DevOps, Server Provisioning, Continuous Build and Deployment {#appendix01-devops-ci}


## User Validation {#appendix01-user-validation}


## Bibliography {#appendix01-bibliography}

### Agile/Lean

* [The Agile Manifesto](http://agilemanifesto.org)
* [Extreme Programming: A gentle introduction](http://www.extremeprogramming.org/)
* [Agile Software Development: A gentle introduction](http://www.agile-process.org/)
* [The Lean Startup by Eric Ries](http://theleanstartup.com/book)
* [Mike Cohn's Scrum and Agile site](http://www.mountaingoatsoftware.com/)
* [Agile @ Adobe Agile Resources](http://blogs.adobe.com/agile/2014/12/05/agile-resources/). Excellent comprehensive list of all kinds of Agile and Scrum Resources
* [Extreme Programming Explained: Embrace Change by Ken Beck](http://www.amazon.com/Extreme-Programming-Explained-Embrace-Change/dp/0321278658/ref=sr_1_1)
* [Agile Software Development with Scrum by Ken Schwaber & Mike Beedle](http://www.amazon.com/dp/0130676349). Original Scrum book.
* [User Stories Applied by Mike Cohn](http://www.amazon.com/User-Stories-Applied-Software-Development/dp/0321205685)
* [How to Manage the "7 Wastes" of Agile Software Development](https://www.scrumalliance.org/community/articles/2013/september/how-to-manage-the-7-wastes%E2%80%9D-of-agile-software-deve)

### Lean UX

* [Lean UX - Applying Lean principles to Improve User Experience by Jeff Gothelf and Josh Seiden](http://www.jeffgothelf.com/blog/lean-ux-book/#sthash.22gOyp12.dpbs)
* [UX for Lean Startups: Faster, Smarter User Experience Research and Design by Laura Klein](http://www.amazon.com/UX-Lean-Startups-Experience-Research/dp/1449334911)

### Kanban

* [Mattias Skarin's Kanban resource page](https://www.crisp.se/gratis-material-och-guider/kanban)
  * [10 kanban boards and their context (Examples](http://blog.crisp.se/2010/12/03/mattiasskarin/1291361993216)
    * [Downloadable PDF](http://blog.crisp.se/wp-content/uploads/2010/12/10-different-kanban-boards-and-their-context.pdf)
* [Leankit's What is Kanban article](http://leankit.com/kanban/what-is-kanban/)
  * [Leankit's Manage Projects with Kanban](http://leankit.com/kanban/online-kanban-board/)
  * [Leankit's 10 kanban boards examples implementation](http://leankit.com/blog/2010/12/10-kanban-boards-leankit-kanban-style/)
  * [LeanKanban University - Definition of Kanban Method](http://www.leankanban.com/node/10)
* [Kanban and Scrum by Henrik Kniberg and Mattias Skarin](http://www.infoq.com/minibooks/kanban-scrum-minibook)

### Content Strategy

#### Content Audits and Inventories

* [Misty Weaver and The Art of Content Audits
Audits, inventories, and the fabulous world of content planning](https://www.lullabot.com/blog/podcasts/insert-content-here/22-misty-weaver-and-art-content-audits)
  * [Misty Weaver, on the web](http://www.meaningandmeasure.com/)
* [Doing Content Inventories by Jeffrey Veen](http://www.adaptivepath.com/ideas/doing-content-inventory/)
* [Drupal Content Audit Module](https://www.drupal.org/project/content_audit)
* [http://growingventuresolutions.com/blog/content-inventory-and-content-audit-views.html

Content Strategy for the Web, by Kristina Halvorson, particularly Chapters 4 and 12

[A Checklist for Content Work by Erin Kissane](http://alistapart.com/article/a-checklist-for-content-work)

The Elements of Content Strategy by Erin Kissane

Information Architecture for the World Wide Web by Peter Morville and Louis Rosenfeld

A Project Guide to UX Design by Russ Unger and Carolyn Chandler

#### Structured Content

Karen McGrane
      http://wimleers.com/article/drupal-8-structured-content-authoring-experience 
Drupalcon Portland 2013 Keynote “Thriving in a world of change”
     http://karenmcgrane.com/2013/05/23/drupalcon-keynote-video-and-talk-notes/
A separate mobile website: no forking way!
     http://www.netmagazine.com/opinions/separate-mobile-website-no-forking-way
Jeff Eaton
Drupalcon Portland 2013 “building for the post-mobile world”
video: https://portland2013.drupal.org/node/1353
slides: https://speakerdeck.com/eaton/building-for-the-post-mobile-world
Larry Garfield
Drupalcon Portland 2013 “Is Drupal a CMS? Do we even know what that means?”
video: https://portland2013.drupal.org/node/3908
slides: http://www.garfieldtech.com/presentations/dcportland2013-is-drupal-cms/#/
Wim Leers
Drupal 8: best authoring experience for structured content?
     http://wimleers.com/article/drupal-8-structured-content-authoring-experience

A Smallcore Manifesto 
Adrian Rossouw
Where do we go from here?
Drupal is not a CMS 
Larry Garfield
COPE: Create Once, Publish Everywhere 
Daniel Jacobson
Content Strategy for Mobile 
Karen McGrane
Adaptive Content Management 
Mark Boulton
Inline Editing and the cost of leaky abstractions 
Jeff Eaton
Content Geography
The Art and Practice of Content Assembly 
Deane Barker

### Core Model

* [Original 2007 presentation by Are Halland: Core+Paths: A Design Framework for Findability, Prioritization and Value](http://www.slideshare.net/aregh/corepaths-a-design-framework-for-findability-prioritization-and-value) (Also see additional recommended slides on Slideshare)
* [The Core Model: Designing Inside Out for Better Results by Ida Aalen](http://alistapart.com/article/the-core-model-designing-inside-out-for-better-results)
  * [The Core Model: Links and Resources](http://alistapart.com/blog/post/the-core-model-links-and-resources)
 