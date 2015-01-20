# Chapter 2. Project Inception. Workflow {#chapter-02}

In this chapter we want to get in the face of the detailed workflow surrounding each of the jobs that need to be done in order to build an initial prototype featuring an MVP vision as preparation for the Project Kickoff that will cut to the core of the project. The Kanban To Do column is filled to the brim with:

* Setup base architecture on the basis of a forked DurableDrupalDistro
* Provisioning for local team VMs
* Create front-end base feature
* Create social networking accounts for use in the prototype 

When these are In Progress, the Welcome Page Feature (including MVP Vision) will be placed in The To Do column.

As each card is placed in the In Progress column (two at any one time given the size of the team and the need for paired development), conversation takes place among the team members and finally the job is confirmed upon acceptance. And the [Kickoff](#chapter-03) will make use of the MVP 1 (prototype) in order to carry out value proposition evaluation. Then, as we drill down into the [Kickoff workflow details](#chapter-04) see how agile's venerable [card, conversation and confirmation](http://xprogramming.com/articles/expcardconversationconfirmation/) branches out into new forms and develops in a much more useful fashion with assumptions discovery and value hypotheses using lean.

Let's peek into the conversations going on around each job.

## Setup base architecture on the basis of a forked DurableDrupalDistro

In order to setup the base architecture for the project, Jake (DevOps) and Jeff (Back end), the job of work mini-team, broke it down into three main tasks:

* Select the frameworks to be used
* Select a usable starter set or distro that can give us a head start using that framework for most of our projects
* Clone that distro for this project

### Frameworks to be used

During the course of the prioritizing of these jobs, which we will see up close in the next chapter dealing with their associated workflow, there were a few heated discussions, on which framework to use for the project, for example, as well as how the team environments should be provisioned.
[Appendix 2. Overcoming Choice Panic. What frameworks should we use?](#appendix-02) thrashes out this important and confusing question. 

> In this appendix we'll be putting Choice Panic behind us and making a firm decision on the CMS framework we'll be using for our content-centric projects. First we'll place all our doubts right on the table for all to see: Should we be using Drupal for this project? really? is Drupal secure after 7.32? What about Backdrop? What about Drupal 8? Should we use that? Then we sift through the options, and choose the best one as our initial hypothesis. In making that decision we'll base ourselves on our current backlog of projects and on the information we actually have to go on right now. And that can change quickly, so we are not married to any framework, we simply want the best tools to get the job done. We'll explore that particular choice and the characteristics that make it the most versatile and dynamic option open to us. We want to be comfortable with the decision, and have the whole team all on the same page.

So for this project, we're going with (Drupal 7)[https://www.drupal.org/start], extended and tailored in the form of a Drupal Distribution.

### Select a usable starter set of distros that can give us a head start using that framework for different kinds of projects

Pair programming discussion:

D> It's important to base your work on a set of [distros](https://www.drupal.org/documentation/build/distributions), one for each kind of project. For example, a general purpose distro, like [Panopoly](https://www.drupal.org/project/panopoly), or our own (DurableDrupalDistro](https://github.com/victorkane/durable-drupal-distro) which has the advantage of sporting a quick, open local [Ansible playbook VM installer](https://github.com/victorkane/ansible-vagrant-durable-drupal-distro right on GitHub), or [Acquia Drupal](https://www.acquia.com/products-services/acquia-drupal), which provides a proprietary one click local stack installer. For ecommerce sites, you should start out with [Commerce Kickstart](https://www.drupal.org/project/commerce_kickstart). 
[COD Conference Organizing](http://usecod.com/), [Acquia Commons for networking sites](http://acquia.com/products-services/acquia-commons-social-business-software), [Open Publish](http://openpublishapp.com/) and [CiviCRM](https://civicrm.org/) are other domain-specific [Drupal distribution](https://www.drupal.org/project/project_distribution) starting points.
D> 
D> All of these should be forked, made your own and should be tailored to your historical and anticipated workflow.

For the DurableDrupal website Jake and Jeff decide to go with our own (DurableDrupalDistro](https://github.com/victorkane/durable-drupal-distro), adopt it as the team's base general purpose distro, and use it for this project.

###  Clone that distro for this project

## Provisioning for local team VMs

Now that we have an initial distro for this project we are ready to provision team member's with Virtual Machines replicating the target production environment, but which will be able to run on their local development environments.

## Create front-end base feature

## Create social networking accounts for the prototype
