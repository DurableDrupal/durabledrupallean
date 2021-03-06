# The DurableDrupal Lean Process Itself {#intro-01}

DurableDrupal Lean is a process factory, providing reusable tools and methods for a team or team of teams within an organization, with the firm purpose of defeating waterfall and guaranteeing delivered value. 

* A process factory
  * Because we don't want to take a rigid scheme and mechanically force ourselves to go through motions that may or may not have anything to do with who we are or what we are trying to accomplish. We want to learn how to create, recreate, evolve and maintain our own process, on every team in our organization, for every different kind of project.
* DurableDrupal Lean
  * We must be in the habit of using upstream Drupal distributions in our organization instead of always starting from scratch. In this book we are providing one, [DurableDistro](https://github.com/DurableDrupal/durable-drupal-distro), along with an Ansible playbook to easily provision it with Vagrant. We think it will give you a great head start and it can be easily curated as needed; and we also list [a lot of the most useful ones out there](#appendix-01-distributions) which you can use for many specialized purposes right off the shelf. The question as always is to stand on the shoulders of giants.
  * Lean: Agile is the new Waterfall. We need Lean, and we want you to know what this software development process is all about and why it should be important to you.
  * See below for explanation of what is Waterfall, Agile, Lean, etc.
* Reusable tools and methods
  * There are various communication methods explained here, like design studio and kickoff meetings. Later on you will make your own. We want to keep it down to a dull roar though, in order to avoid top heavy, documentation laden wastes of time.
  * Lean UX problem statement and hypotheses templates.
  * Automated provisioning using Vagrant, VirtualBox and Ansible
  * Continuous integration adding Jenkins into the mix
  * Continuous delivery to staging and live environments
* For a team or team of teams.
  * We are talking continuous improvement in your organization, whether it's a one man shop (still a team!), an agency or company department with a single team, or a team of teams (we never want to work on a scale bigger than a team when we focus on work in progress). We are talking everyone face to face in a single building, or a world-wide distributed team or team of teams. 
  * We are talking continuous improvement in the organization as curated evolution of process and tools. Delivered and tested feature retrospectives keep the best for re-use, look for better ways, extend lessons learned to other teams.
* Defeating waterfall
  * Great success comes from great failures. Even the failures may have looked like a good idea at the time. But we want to prevent failure and encourage success. We really want to be able to deliver the best we have. So we must learn to fit productively with the process and evolve that process.
* Guaranteeing delivered value
  * Because code can no longer be implemented on the basis of "functional requirements". Code's sole purpose in living is to be able to test a hypothesis envisioning value to be obtained by the client as a result of its existence. Code should be designed as such, and tested as such. Becuase neither is it enough to test code and be satisfied that it works as advertised in order to consider a job of work completed. The functionality designed to give value must be tested to make sure it actually delivers that expected value to the client. This is at the core of Lean and we'll be sure to drill down here.

## A very short history of modern software development process

Why use process at all? Well, work is social in nature, ever since we humans gained an opposable thumb. And it always exists in an historical context. So we engineer things using today's tools and processes in order to avoid making the same expensive mistakes over and over again, and in order to avoid inventing the wheel every time we tool up for a product.

We need process to avoid wasting time, money and resources. To avoid failing. Again and again. Let's examine a very short history of modern software development process to understand fully why Lean is essential.

## The limitations of Waterfall and Agile for Web development

The much criticized [Waterfall Model](http://en.wikipedia.org/wiki/Waterfall_model) is a sequential process for software development "in which progress is seen as flowing steadily downwards (like a waterfall) through the phases of Conception, Initiation, Analysis, Design, Construction, Testing, Production/Implementation and Maintenance." Each phase corresponds to an autonomous silo which receives its input from the previous silo and performs additional work according to its particular discipline. So outputs are handed off in sequence from one discipline "silo" to another. It is no accident that this method, which at least raised software development from the level of artesanal improvisation to that of engineering, had its origins in the highly structured manufacturing and construction industries.

But in the eighties a study carried out by the US Air Force (Development of an Environment for Software Reliability - http://www.dtic.mil/cgi-bin/GetTRDoc?Location=U2&doc=GetTRDoc.pdf&AD=ADA256609) discovered that the use of the Waterfall model results in a very high rate of project failure.

[Agile software development methodologies](http://en.wikipedia.org/wiki/Agile_software_development), on the other hand, favor an iterative and incremental approach due to the following shortcomings evidenced by the Waterfall Model:

* A minimum of 40% in change requests take place during project life-cycle, making it impossible for each discipline to  complete its work and then hand-off a perfect output to the next discipline in line: discipline silos having already "finished" their work will have to do it all over again to comply with those changes, and the impact may vary widely. For example, the design and even the candidate architecture may have to be completely re-done.
* Clients often need to see working prototypes at various stages in order to properly finalize their requirements, so that Construction cannot be carried out in one fell swoop without a series of programmed opportunities for user feedback.
* Design may dictate solutions impossible or very difficult to implement, which can only be seen during the Construction phase. In other words, a lot of design and construction work may have to be thrown away and started over.
* By the same token, design may be dictated by stakeholders who are unaware of the full benefits of the technology, and only become aware as Construction progresses, which is one of the principle sources for the high rate of change requests in most projects.

Diserée Sy's article [Adapting Usability Investigations for Agile User-centered Design](http://uxpajournal.org/wp-content/uploads/pdf/agile-ucd.pdf), published in 2007, first introduces the characteristics of both the Waterfall and Agile software development methodologies, contrasts the benefits of Agile to the deficiencies of Waterfall, and then goes on to enumerate certain "adaptations to the timing, granularity, and reporting used for Agile interactive usability investigations, with an intended audience of usability practitioners."

The [Rational Unified Process](http://en.wikipedia.org/wiki/Rational_Unified_Process) (más tarde comprado por IBM) first, and [Agile](http://en.wikipedia.org/wiki/Agile_software_development) later on, as seen in the diagram below taken from the 2007 Desirée Sy article, replace the waterfall with a sequence of mini-waterfalls, which at least offer more feedback before each more frequent delivery.

Agile is an improvement over Waterfall since the abyss separating requirements gathering from testing is shorter and since the mini-cycles allow for more cross-collaboration, testing and feedback. This can be seen in the following diagram from the article:

![Waterfall and Agile](images/sy-waterfall-agile.png)

(Note: This author signed, in mid-2006, the [Agile Manifesto](http://www.agilemanifesto.org/) que este autor firmó [en mediados de 2006](http://www.agilemanifesto.org/sign/display.cgi?ms=000000067)).

> "However, this meant that we needed to find a way to conduct usability tests, interviews, and contextual inquiry—both in the lab and the field—within an Agile framework. To achieve this, we adjusted the timing and granularity of these investigations, and the way that we reported our usability findings. This paper describes our main adaptations." 
> 
> "It is possible to use the familiar arsenal of usability investigation methods on Agile (and other iterative development) projects, including formative usability testing, user and task analysis, interviews, and even field-based work like contextual inquiry. This is achieved by changing the timing and granularity of the investigations, and how results are reported."

In the article, Sy and Miller describe in detail the method they developed for integrating Agile with user-centered design.

## Improving Agile with Cycle 0 and Staggered Sprints

The solution resided in a technique called Cycle 0 (sometimes called Sprint 0 or Staggered Sprints), in which design activity takes place one sprint ahead of development. Work is designed and validated during the “design sprint” and then passed off into the development stream to be implemented during the development sprint. 

![Cycle 0 with Staggered Sprints](images/sy-miller-staggered-sprints.jpg)

> "To allow the User Experience Team to iterate on designs, we usability tested prototypes at least one cycle ahead of developers, and then passed on the validated designs to be implemented. We would also conduct contextual inquiry for workflows at least two cycles ahead, and usability test the implemented working version to check for design drift."

## Achieving a still better process with Lean UX and Design + Dev

> "Many teams have misinterpreted this model. Sy and Miller always advocated strong collaboration between designers and developers during both the design and development sprints. Many teams have missed this critical point and have instead created workflows in which designers and developers still communicated by handoff, creating a kind of mini-waterfall process within the agile cycles." (From *Gothelf, Jeff (2013-02-22). Lean UX: Applying Lean Principles to Improve User Experience, O'Reilly Media)*

What occurs is that even when cross collaboration is encouraged, with staggered sprints it becomes very easy for the entire team to never be working on the same thing at the same time. You never realize the benefits of cross-functional collaboration because the different disciplines are most often focused on different things. Also, when two-week sprints are used in a Scrum context, designers do not get enough creative time.

As a result it's necessary to go beyond staggered sprints.

![Building Lean UX into the Rhythm of Scrum](images/gothelf-lean-plus-scrum.jpg)

First of all, themes allow for several scrums to be united under the same umbrella, giving time for greater creativity on the part of graphic design and user experience team members, and "the entire team is working on the same thing at the same time".

Each theme, and indeed each sprint, is kicked off with a series of brainstorming and validation exercises with the participation of the whole team (light green). The resulting ideas and sketches are taken to the traditional sprint planning meeting, where again the whole team participates in a process of writing user stories, and then evaluating and prioritizing them to form the sprint backlog (purple).

Then, weekly user validation sessions are added in (blue-green), so that the ideas being implemented can be subject to testing for usability and value.

See also [Beyond Staggered Sprints: How TheLadders.com Integrated UX into Agile](http://johnnyholland.org/2010/10/beyond-staggered-sprints-how-theladders-com-integrated-ux-into-agile/).
  
## The Best Process we Know: Design + Dev + DevOps

DurableDrupal Lean adds DevOps into the mix. Just as it is critical for cross-collaboration between design and development, so it is just as critical for there to be cross-collaboration between design, development and DevOps, both in provisioning so that the team can really work in parallel, as well as in building, feedback conversations, testing, continuous integration and deployment.

## Waste that is eliminated by using DurableDrupal Lean

Waste is of course, the opposite of value. When Agile and Lean processes are absent in a project the probability of it occurring is very high. Possible causes of waste in software development: 

1. Unfinished work left rotting in isolated silos This can occur as a result of incomplete stories having been prioritized, of technical complexity that was not analyzed correctly during planning, postponed tasks blocking progress with a story, unavailable dependencies, or making developers leave an unfinished story and start another one.
1. Feature creep without validating for impact or value. This will always happen unless it is combated; sometimes the developers "gold-plate" the backlog with things no-one even needs.
1. Isolated silos keep on re-inventing the wheel due to a lack of proper knowledge-sharing among members of the team or teams.
1. Handoffs chronically disrupts workflow
1. Delays because isolated silos and teams missing skills
1. Task switching because work overload and broken workflow
1. Many defects also arise as a result of chaotic focus and blocked knowledge sharing

See [How to Manage the "7 Wastes" of Agile Software Development](https://www.scrumalliance.org/community/articles/2013/september/how-to-manage-the-7-wastes%E2%80%9D-of-agile-software-deve).

## Bibliography {#intro-01-bibliography}

In this book we place the bibliography at the front, so you can become familiar with the resources you want to explore first.

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
* A big proponent of style guides in the Drupal Community, including setting up automated style guides, is [John Albin](https://www.drupal.org/u/johnalbin). See for example [Style Guide Driven Development](https://melbourne2015.drupal.org.au/session/style-guide-driven-development):
  * Automated style sheet guide [KSS-node](github.com/kss-node/kss-node)

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
 
### PHP Renaissance

* [Downlowd current stable PHP](http://php.net/downloads.php)
* [PHP The Right Way](http://www.phptherightway.com/)
  * [Free book](https://leanpub.com/phptherightway)
* [PHP must watch resource list](https://github.com/phptodayorg/php-must-watch) 
* [Modern PHP](https://github.com/codeguy/modern-php)
* [Modern Application Development with PHP](https://leanpub.com/modern-application-development-with-php)
* [No framework tutorial](https://github.com/PatrickLouys/no-framework-tutorial)
