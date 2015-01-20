# Chapter 2. Project Inception. Workflow {#chapter-02}

In this chapter we want to get in the face of the detailed workflow surrounding each of the jobs that need to be done in order to build the initial prototype featuring an MVP vision as preparation for the Project Kickoff that will cut to the core of the project. The Kanban To Do column is filled to the brim with:

* Setup base architecture on the basis of a forked DurableDrupalDistro
* Provisioning for local team VMs
* Create front-end base feature
* Create social networking accounts for use in the prototype 

When these are In Progress, the Welcome Page Feature (including MVP Vision) will be placed in The To Do column.

As each card is placed in the In Progress column (two at any one time given the size of the team and the need for paired development), conversation takes place among the team members assigned to the job, which is finally confirmed upon acceptance and moved to the MVP 1 column. And the [Kickoff](#chapter-03) will make use of the MVP 1 (prototype) in order to carry out value proposition evaluation. Then, we'll drill down into the [Kickoff workflow details](#chapter-04) and see how agile's venerable [card, conversation and confirmation](http://xprogramming.com/articles/expcardconversationconfirmation/) branches out into new forms and develops in a much more useful fashion with assumptions discovery and value hypotheses using DurableDrupal Lean.

Let's peek into the conversations going on around each MVP 1 job so we can get at the details.

## Setup base architecture on the basis of a forked DurableDrupalDistro

In order to setup the base architecture for the project, Jake (DevOps) and Jeff (Back end), the job of work mini-team, broke it down into three main tasks:

* Select the frameworks to be used
* Select a usable starter set or distro that can give us a head start using that framework for most of our projects
* Clone that distro for this project

### Frameworks to be used

Jeff has drawn up a summary of their discussion entitled [Overcoming Choice Panic. What frameworks should we use?](#appendix-02) in which they thrash out this important and sometimes confusing question.

> We are putting Choice Panic behind us and making a firm decision on the CMS framework we'll be using for our content-centric projects. First we'll place all our doubts right on the table for all to see: Should we be using Drupal for this project? really? is Drupal secure after 7.32? What about Backdrop? What about Drupal 8? Should we use that? Then we sift through the options, and choose the best one as our initial hypothesis. In making that decision we'll base ourselves on our current backlog of projects and on the information we actually have to go on right now. And that can change quickly, so we are not married to any framework, we simply want the best tools to get the job done. We'll explore that particular choice and the characteristics that make it the most versatile and dynamic option open to us. We want to be comfortable with the decision, and have the whole team all on the same page.... [Read on](#appendix-02)!

So for this project, we're going with (Drupal 7)[https://www.drupal.org/start], extended and tailored in the form of a Drupal Distribution.

### Select a usable starter set of distros that can give us a head start using that framework for different kinds of projects

Job discussion:

D> It's important to base our work on a set of [distros](https://www.drupal.org/documentation/build/distributions), one for each kind of project. For example, a general purpose distro, like [Panopoly](https://www.drupal.org/project/panopoly), or our own (DurableDrupalDistro](https://github.com/victorkane/durable-drupal-distro) which has the advantage of sporting a quick, open local [Ansible playbook VM installer](https://github.com/victorkane/ansible-vagrant-durable-drupal-distro right on GitHub), or [Acquia Drupal](https://www.acquia.com/products-services/acquia-drupal), which provides a proprietary one click local stack installer. For ecommerce sites, we would start out with [Commerce Kickstart](https://www.drupal.org/project/commerce_kickstart). 
[COD Conference Organizing](http://usecod.com/), [Acquia Commons for networking sites](http://acquia.com/products-services/acquia-commons-social-business-software), [Open Publish](http://openpublishapp.com/) and [CiviCRM](https://civicrm.org/) are other domain-specific [Drupal distribution](https://www.drupal.org/project/project_distribution) starting points.
D> 
D> All of these should be forked, made our own and should evolve as they are tailored to the projects we are and will be working on.

For the DurableDrupal website Jake and Jeff decide to go with our own (DurableDrupalDistro](https://github.com/victorkane/durable-drupal-distro), adopt it as the team's base general purpose distro, and use it for this project.

###  Clone that distro for this project

Let's clone the distro to our own GitHub organization, where we can curate it for our own purposes and fork it individually for each project that comes up and requires a general purpose distro.

## Provisioning for local team VMs

Now that we have an initial distro for this project we are ready to provision team member's with Virtual Machines replicating the target production environment, but which will be able to run on their local development environments.

## Create front-end base feature

## Create social networking accounts for the prototype
