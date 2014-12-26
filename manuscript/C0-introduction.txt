# Introduction {#chapter-00}

## Tool up for solid web apps now and maintain them for years with a powerful Drupal distro

This book is for web app development teams, called upon by their clients to move their business model to the internet, their back-office to the cloud.

This book will empower you and your team, no matter what your level of expertise, to simplify the building of solid solutions for your clients' real needs, and to facilitate in a productive and cost-effective manner the maintenance these solutions will be crying out for from the moment they are born.

In the process, you will actually be evolving for yourselves a lean web factory to output durable solutions that can be maintained for years to come.

## Change, maintenance, continous delivery and the long haul

Successful web developers and agencies know that the real challenge is how to embrace continuous innovation and delivery throughout the web app life cycle.

**Delivering websites and web apps is only the beginning. The real question for success in web development is how to continue to ply your client with continual fixes and releases in order to fix problems and satisfy change requests, to optimize value at all times.**

Because constant change is inevitable, and ever-present throughout the web app life-cycle: 

* First in the minimum of 40% in changes that will be requested in the weeks or months of development.
* Secondly, in the feature and usability requests the solution will have to assimilate in order to maintain its value over time.
* Thirdly in the security threats that will have to be dealt with in as fully an automated way as possible.
* Fourthly in the architectural and deployment changes that will be required as time goes by, in the struggle to scale with growth and cut costs with new technological breakthroughs.

Because it's not about the "single click site generation" and easy scaffolding any decent framework or "hosting" solution offers. We'll soon see how to fire up a framework in seconds, in just a few clicks, but the devil is in how we empower ourselves with a process that is going to facilitate, stabilize and simplify our work in the face of this constant change. By using the most exciting best of breed industry standard tools, like Ansible, Vagrant and Docker, Cloud-based hosting, and the all important Git branch model; just to mention a few of the things we will be working with here.

The theme of embracing change, while not new at all, marks the difference between success and failure, is born of the inevitable failures as well as the successes we all live through as we gain experience, and runs throughout the book so that web development can be fun instead of being a constant source of stress, code and maintenance debt.

We're here for the long haul.

And we're using [Drupal](https://www.drupal.org/) now.

And we're using Lean process now. 

## Overview of Book Contents

So here's what we'll be doing:

* Chapter 1: First Lean DurableDrupalDistro Project
  * First meeting with the client

* Chapter 2: Setting up just enough shop to deliver our first web app
  * Team consciousness: client reps and dev team together
  * Shop infrastructre
    * Central code repos for all deliverables using the Git branching model
    * VPS MVP instances
      * Testing & Integration instance
      * Staging instance
      * Production ready instance  
    * Every team member has their own dev environment automatically provisioned on their own laptop
    * Tools for running our agile developoment process
  * Fork the distro and make it our own
  * User stories and doing it with agile
  * Delivery as client empowerment
  * Retrospective: We did it! But...
    * Agile is the new waterfall (pixel perfect design -> "implementation")
    * Team (devs and designers, devs and client reps) couldn't really work in parallel
      * The tangle of User Stories and Design
    * Client took delivery of a monolithic blob he wasn't sure how to use
      * We had to do special training (not to mention train the trainers)
      * Client reps began a slew of change requests that could have come earlier if they had been familiar with the system
    
* Chapter 2: Pain driven development
  * New project!
  * Value hypotheses
  * Design studio for nerds... and for the client too
  * Getting the team working in parallel
  
* Chapter 3: MVP prototypes

* Chapter 4: Grabbing the legacy content
This should be postponed for migrations book

* Chapter 5: Candidate architecture
  * Choices panic: see Appendex 1 xxxxxx
  * We're evolving on top of best of breed

* Chapter 6: Build the recursive MVP of MVP's
  * Every user story is an MVP
  * No project is ever anything more than an MVP
  
* Chapter 7: Go team test team go go go
    The advantage of using frameworks isn't just that they're tried and tested, but that they empower testing and TTD
    
* Chapter 8: Build, deploy, maintain
  * Rinse and repeat over "development"

* Appendix 1: Overcoming Choice Panic - What frameworks should we use?
  
    We need to free ourselves from choice panic which can paralyze us or disrupt our work. Dialog is necessary to ensure that the project stakeholders (all of them) are on board with the major framework optionss. We need to have this discussion sooner rather than later in order to share a common perspective and be ready to get down to work. In order to achieve this, we will be facing some tough questions together:
    
  * Building from scratch or not? Frameworks or not?
  * Proprietary or not? Open-source or not?
  * WordPress or not?
  * Drupal or not?
  * Drupal 8 or not?
  * Backdrop or not?
  * Vanilla Drupal 7 or not? Distro or not?
  * Presenting DurableDrupalDistro: fork it, tailor it, maintain it, branch and release it over all your projects!
  * Preparing to migrate gradually all along, so we'll be ready when the time comes
 
 * Appendix 2: Team Workflow and Provisioning

## Formatting Conventions

This book follows [industry standard formatting and typographical conventions](https://leanpub.com/help/manual) for web development books. 

## Obtaining and using the DurableDrupalDistro and other code examples

This is a book we need to work through together, so a starter Drupal Distro has been provided. 

> For team dev, integration, staging and production DurableDrupalDistro provisioning, fork and adapt (or directly download and use) the [Ansible playbook for setting up Durable Drupal Distro](https://github.com/victorkane/ansible-vagrant-durable-drupal-distro).

> Or grab the [DurableDrupalDistro](https://github.com/victorkane/durable-drupal-distro) itself and build out as you like.

### At a minimum

Thanks to all the modern tools that have come along, all you really need is a laptop with some disk space and a decent amount of RAM. And we promise not to dirty it up with a lot of "server" stuff, thanks to Vagrant, Virtual Box, Ansible and Docker. We'll be setting up complete self-contained server replicas that won't affect your regular configuration at all. And you'll be able to follow through all the examples throughout the book.

## Contact and feedback
Victor Kane…
Book page...
mailing lists

## Acknowledgements


But more than a book this is a community of teams. Dive in!
