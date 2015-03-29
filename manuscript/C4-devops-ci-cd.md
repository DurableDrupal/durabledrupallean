# Chapter 4. DevOps. Continuous Integration and Continuous Delivery {#chapter-04} 

## Resources for Server Provisioning and Deployment

Here is a short list of the many available resources for the all important question of server provisioning and deployment automation for frequent and continuous build and continuous delivery approaches. Without such automation on some level team paralysis, delays and workflow blowup will haunt us as the handoff monster rears its ugly default waterfall head throughout the project.

* [Jeff Geerling's book Ansible for DevOps: Server Configuration Management for humans](https://leanpub.com/ansible-for-devops)
  * [GitHub Repo for the book (very actively kept up-to-date)](https://github.com/geerlingguy/ansible-for-devops)
  * [Jeff's Austin DrupalCon presentation DevOps for Humans - Ansible for Drupal Deployment Victory!](https://austin2014.drupal.org/session/devops-humans-ansible-drupal-deployment-victory.html)
    * [Slides](http://www.slideshare.net/geerlingguy/devops-for-humans-ansible-for-drupal-deployment-victory)
  
* DigitalOcean tutorial [How To Create an Ansible Playbook To Automate Drupal Installation on Ubuntu 14.04](https://www.digitalocean.com/community/tutorials/how-to-create-an-ansible-playbook-to-automate-drupal-installation-on-ubuntu-14-04)

## Continuous Integration and Continuous Delivery

For true team cross-collaboration to exist we'd better have enough feedback on changes to the codebase and on deployment to environments. And that includes automated feedback. In a nutshell we are actually talking about ALM: Application Lifecycle Management.

These may be evolving terms, but if we're using them (and we are) we'd better get them straight. Bryan Root makes [a good distinction](http://blog.nwcadence.com/continuousintegration-continuousdelivery/):

> "So what is CI?  In short, it is an integration of code into a known or working code base.... The top benefits are to provide fast feed back to the members of the team and to ensure any new changes don’t break the working branch."
>
> "CD... is an automated process to deliver a software package to a environment.... we can now extend the fast feedback loops and reduction of constraints with packaging techniques, automation workflows, and integrated tools that keep track of the software versions in different environments."
>
> " CI and CD are two completely separated practices that are tightly interlocked to create a unified ALM workflow."

So, it's not just tools, the question is for the following feedback to be available: on the one hand, build and automated test results, and on the other, application status upon deployments of new features to environments (i.e., development/integration, staging, live). 
