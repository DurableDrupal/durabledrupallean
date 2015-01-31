# Appendix 3. Team Workflow and Provisioning {#appendix-03}

## Team roles

Basing ourselves on [Web Style Guide by Patric J. Lynch and Sarah Horton](http://webstyleguide.com/wsg3/1-process/2-development-team.html), published a few years ago in 2009 by Yale University Press. At that point, the traditional Website development team core skillset were presented as being:

* Strategy and planning
* Project management
* Information architecture and user interface design
* Graphic design for the web
* Web technology
* Site production

with Web Team roles and responsibilities being:

* Project stakeholder or sponsor
* Web project manager
  * Account executive
  * Quality assurance tester
* Usability lead
* Information architect
* Art director
  * Web graphic designer
  * Interactive designer (Flash, JavaScript, Ajax)
  * Media specialist (photography, illustration, audiovisual, Adobe Flash)
* Web technology lead
  * Web application programmer (.Net, Java, php/Perl, Ruby)
  * Web page engineer (xhtml, css, JavaScript, Ajax)
  * Database administrator
  * Web systems expert or webmaster
* Site production lead
  * html page coder
* Site editor
 * Site copywriter
 * Content domain expert (content coordination, research)

TODO Translate this in steps to our current team role set introduced in [Chapter 1](#).

## Basic team workflow
clone
pull, branch, work, pull request
rinse and repeat

"We'll first show you [how to set up a workspace](a_workspace_in_a_lamp_stack.html), getting a folder somewhere you can configure as a Drupal doc root, that is, the main Drupal directory that can be picked up by a LAMP stack and made available to a browser as a URL.

This can be done on a dedicated server, on a VPS, on a virtual machine or directly on your laptop, even on a good shared hosting, but you've got to have ssh access to the command line.

We all need to be able to do this no matter what our role on the team, so we'll show you a couple of examples.

Then we'll see [how to grab our very own DurableDrupalDistro and fire it up](obtaining_and_installing_the_durabledrupaldistro.html).

Finally, we'll [check out what we have going for us](whats_included_in_durabledrupaldistro.html) under the hood right off-the-shelf, we'll [take our first steps](durabledrupaldistro_first_steps.html), and then I'll give an example of [updating and maintaining the distro itself](updating_durabledrupaldistro_itself.html)".

## Getting a workspace in a LAMP stack

El Viejo shows here how to set up a workspace from scratch, in his usual opinionated fashion.

* on a [VPS](#vps) like Linode or Digital Ocean,
* on personal laptop/workstation alternatives
  * [Water Works stack](#water-works-stack)
  * [Bitnami](#bitnami)
    * Drupal App
    * Drupal Server
  * [Kalabox](#kalabox)
* [Roll your own](#roll-your-own)
* on a [shared hosting account](#shared-hosting-account) with command line access and drush

### VPS
TODO linode

TODO digital ocean

### Water Works stack

Well, Water Works never got around to offering one, or else they did and then started charging for it, so nobody used it and it died. But Acquia has one! Very convenient for running Drupal apps on your laptop, but it isn't a virtual machine, it's an app only, so that means that while you can run it and everything, it doesn't emulate the target live environment (a GOOD idea) the app will be running on when it is launched. Get it [here](http://www.acquia.com/downloads).

### Bitnami

[Bitnami](https://bitnami.com/stack/drupal) swings both ways, with the app approach and the VirtualBox VM alternative (recommended but [a lot of work](http://awebfactory.com/node/524) and then [more work](http://awebfactory.com/node/525)).

### Pantheon
Single click .....

And you can have the best of both worlds, with pantheon in the cloud and on your desk... Kalabox!

### Kalabox

Ah, the amigos at [Kalamuna](http://www.kalamuna.com/) are a breath of fresh air. They've not only come up with [Kalabox](http://www.kalamuna.com/products/kalabox) but are now developing [Kalabox 2](https://github.com/kalabox), the [NodeWebkit](https://github.com/rogerwang/node-webkit) and [Docker](https://www.docker.com/) wonder, as a completely open source project after a successful [Kickstarter campaign](https://www.kickstarter.com/projects/kalabox/kalabox-advanced-web-tools-for-the-people).

I've tried it out quite a bit. See [how I installed Kalabox 1](http://awebfactory.com/node/522) and used it as a Pantheon workflow solution. Integration with [Pantheon hosting](https://www.getpantheon.com/) and their one-click Drupal Distro site builder is a hallmark of Kalabox 1. Very useful considering its [revolutionary architecture](https://www.getpantheon.com/how-it-works) and [standardizing workflow](https://www.getpantheon.com/how-it-works) (at least as far as Drupal hosting is concerned). Alternative hosting support plug-ins are expected with Kalabox 2.

### Ansible
(study up on Ansible for Dev-Ops book first! buy the bundle!)
* Ansible on a Mac to run a server
* Ansible on a Mac to run a local vagrant/vbox instance

 




### Roll your own
sthg about virtual box & vagrant, with puppet, chef, ansible...

### Shared hosting account
We shouldn't even be talking about this, but recent improvements in shared hosting accounts have made something like a reseller account somewhat (only just) viable, at least for hosting small to middling projects.

First thing to do is get Drush on there, once you've gotten ssh command-line access, if you can't get that switch hosting now (and if you're even reading this section, second thing is to create a subdomain for each site: don't go running Drupal from a sub-directory).

## Bringing the whole team up with the DurableDrupalDistro

## What's included in DurableDrupalDistro

## DurableDrupalDistro for our first project

So we're in oue workspace, let's say on a VPS.

### What we want to do

* Create virtual host
* Create database
* Clone and set up distro
* Install with drush on the command line
* Check it out

#### Create virtual host



#### Create database
#### Clone and set up distro
#### Install with drush on the command line
#### Check it out

## Updating DurableDrupalDistro itself

~~~~~~~~
$ drush pm-refresh
Refreshing update status information ...
Done.
$ drush pm-update
 Name                 Installed  Proposed  Message
                      Version    version
 Drupal               7.31       7.32      SECURITY UPDATE available
 Calendar (calendar)  7.x-3.4    7.x-3.5   Update available
 CKEditor (ckeditor)  7.x-1.15   7.x-1.16  SECURITY UPDATE available
 Profiler Builder     7.x-1.1    7.x-1.2   Update available
 (profiler_builder)


Update information last refreshed: Tue, 10/21/2014 - 13:20
NOTE: A security update for the Drupal core is available.
Drupal core will be updated after all of the non-core projects are updated.

Security and code updates will be made to the following projects: Calendar [calendar-7.x-3.5], CKEditor - WYSIWYG HTML editor [ckeditor-7.x-1.16], Profiler Builder [profiler_builder-7.x-1.2]

Note: A backup of your project will be stored to backups directory if it is not managed by a supported version control system.
Note: If you have made any modifications to any file that belongs to one of these projects, you will have to migrate those modifications after updating.
Do you really want to continue with the update process? (y/n):
Project calendar was updated successfully. Installed version is now 7.x-3.5.
Backups were saved into the directory                                [ok]
/home/drupallean/drush-backups/drupal_lean/20141021132817/modules/calendar.
Project ckeditor was updated successfully. Installed version is now 7.x-1.16.
Backups were saved into the directory                                [ok]
/home/drupallean/drush-backups/drupal_lean/20141021132817/modules/ckeditor.
Project profiler_builder was updated successfully. Installed version is now 7.x-1.2.
Backups were saved into the directory                                [ok]
/home/drupallean/drush-backups/drupal_lean/20141021132817/modules/profiler_builder.

Code updates will be made to drupal core.
WARNING:  Updating core will discard any modifications made to Drupal core files, most noteworthy among these are .htaccess and robots.txt.  If you have made any modifications to these files, please back them up before updating so that you can re-create your modifications in the updated version of the file.
Note: Updating core can potentially break your site. It is NOT recommended to update production sites without prior testing.

Do you really want to continue? (y/n):
Project drupal was updated successfully. Installed version is now 7.32.
Backups were saved into the directory                                [ok]
/home/drupallean/drush-backups/drupal_lean/20141021132817/drupal.
No database updates required                                         [success]
'all' cache was cleared.                                             [success]
Finished performing updates.                                         [ok]
$ git status
$ git add .
$ git commit -am "Maintenance update to drupal core 7.34 plus updated contrib modules"
$ git push
$ git tag
$ git tag -a "December2014" -m "Maintenance core and contrib update"
$ git push --tags
~~~~~~~~

Now we need to prepare the site (see [Quick install for developers (command line)](https://www.drupal.org/documentation/install/developers)

    cp sites/default/default.settings.php sites/default/settings.php

Give the web server write privileges (666 or u=rw,g=rw,o=rw) to the configuration file.

    chmod a+w sites/default/settings.php

Give the web server write privileges to the sites/default directory.

    chmod a+w sites/default

so we can re-install from scratch to test. Check out incredible options available with drush help:

~~~~~~~~
$ drush help site-install
Install Drupal along with modules/themes/configuration using the specified
install profile.

Examples:
 drush site-install expert --locale=uk     (Re)install using the expert install
                                           profile. Set default language to
                                           Ukranian.
 drush site-install                        Install using the specified DB
 --db-url=mysql://root:pass@localhost:por  params.
 t/dbname
 drush site-install                        Install using SQLite (D7+ only).
 --db-url=sqlite://sites/example.com/file
 s/.ht.sqlite
 drush site-install --account-name=joe     Re-install with specified uid1
 --account-pass=mom                        credentials.
 drush site-install standard               Pass additional arguments to the
 install_configure_form.site_default_coun  profile (D7 example shown here - for
 try=FR                                    D6, omit the form id).
 my_profile_form.my_settings.key=value
 drush site-install                        Disable email notification during
 install_configure_form.update_status_mod  install and later. If your server
 ule='array(FALSE,FALSE)'                  has no smtp, this gets rid of an
                                           error during install.

Arguments:
 profile                                   the install profile you wish to run.
                                           defaults to 'default' in D6,
                                           'standard' in D7+
 key=value...                              any additional settings you wish to
                                           pass to the profile. Fully supported
                                           on D7+, partially supported on D6
                                           (single step configure forms only).
                                           The key is in the form [form
                                           name].[parameter name] on D7 or just
                                           [parameter name] on D6.

Options:
 --account-mail                            uid1 email. Defaults to
                                           admin@example.com
 --account-name                            uid1 name. Defaults to admin
 --account-pass                            uid1 pass. Defaults to a randomly
                                           generated password. If desired, set
                                           a fixed password in drushrc.php.
 --clean-url                               Defaults to 1
 --db-prefix                               An optional table prefix to use for
                                           initial install.  Can be a key-value
                                           array of tables/prefixes in a
                                           drushrc file (not the command line).
 --db-su=<root>                            Account to use when creating a new
                                           database. Must have Grant permission
                                           (mysql only). Optional.
 --db-su-pw=<pass>                         Password for the "db-su" account.
                                           Optional.
 --db-url=<mysql://root:pass@host/db>      A Drupal 6 style database URL. Only
                                           required for initial install - not
                                           re-install.
 --locale=<en-GB>                          A short language code. Sets the
                                           default site language. Language
                                           files must already be present. You
                                           may use download command to get
                                           them.
 --site-mail                               From: for system mailings. Defaults
                                           to admin@example.com
 --site-name                               Defaults to Site-Install
 --sites-subdir=<directory_name>           Name of directory under 'sites'
                                           which should be created. Only needed
                                           when the subdirectory does not
                                           already exist. Defaults to 'default'

Aliases: si
~~~~~~~~

So let's install in Spanish, specifying db credentials, uid1 user name and password, uid1 user email, site email and site name

~~~~~~~~
site-install drupallean --locale=es --db-url=mysql://drupal_lean:lean@localhost/drupal_lean --account-name=admin --account-pass=omg --account-mail=victorkane@gmail.com --site-mail=drupallean@awebfactory.com.ar --site-name=DrupalLean

You are about to DROP all tables in your 'drupal_lean' database. Do you want to continue? (y/n): y
No tables to drop.                                                   [ok]
Starting Drupal installation. This takes a few seconds ...           [ok]
WD php: Warning: Invalid argument supplied for foreach() in          [warning]
_features_restore() (line 966 of
/home/drupallean/drupal-lean/sites/all/modules/contrib/features/features.module).
Installation complete.  User name: admin  User password: omg     [ok]
~~~~~~~~



## Updating DurableDrupalDistro itself redux {#appendix-03-update-distro}

TODO Ansible operations playbook or role or whatever to do this on any server

### Clone

    $ git clone git@github.com:DurableDrupal/durable-drupal-distro.git

### Install

#### Create virtual host for this instance

Step into the cloned distro directory and grab document root path

    $ cd durable-drupal-distro/
    $ pwd
    /home/drupallean/durable-drupal-distro

Create an Apache HTTP Server sites-available file for all DurableDrupal instances: 

    $ sudo vi /etc/apache2/sites-available/durabledrupal

Add the following text:

˜˜˜˜˜˜˜˜
<VirtualHost *:80>
 ServerName durable-drupal-distro.awebfactory.net
 DocumentRoot /home/drupallean/durable-drupal-distro
 <Directory "/home/drupallean/durable-drupal-distro">
   Options Indexes FollowSymLinks MultiViews
   AllowOverride All
 </Directory>
</VirtualHost>
˜˜˜˜˜˜˜˜

Register with Apache Server and reload configuration to enable virtual host:

˜˜˜˜˜˜˜˜
$ sudo a2ensite durabledrupal
Enabling site durabledrupal.
To activate the new configuration, you need to run:
  service apache2 reload
$ sudo service apache2 reload
 * Reloading web server config apache2                                   [ OK ]
˜˜˜˜˜˜˜˜

#### Set up instance database

Create MySql database for the instance, say database ddd with db user ddd and password dddpw22, either following instructions in ./INSTALL.mysql.txt or else with something like [Phpmyadmin](https://www.digitalocean.com/community/tutorials/how-to-install-and-secure-phpmyadmin-on-ubuntu-14-04).

#### Configure file permissions

Set up everything required to install from the command line with [drush](http://www.drush.org/en/master/), the Drupal shell. The following procedure is [idempotent](http://en.wikipedia.org/wiki/Idempotence#Computer_science_meaning) (will produce the same results if executed multiple times) and will consequently work for a fresh install or in order to zap an existing site and start over. See [Quick install for developers (command line)](https://www.drupal.org/documentation/install/developers) for more details.

First zap or create the Drupal settings.php file:

    $ cp sites/default/default.settings.php sites/default/settings.php

Give the web server write privileges (666 or u=rw,g=rw,o=rw) to the configuration file.

    $ chmod a+w sites/default/settings.php

Give the web server write privileges to the sites/default directory.

    $ chmod a+w sites/default

If there is no sites/default/files directory create it, then:

    sudo chown -R www-data sites/default/files
    sudo find sites/default/files -type d -exec chmod 775 {} \; 
    sudo find sites/default/files -type f -exec chmod 664 {} \; 

#### Install Drupal site from the command line with drush

Continuing in the document root and execute the following command:

~~~~~~~~
$ drush si drupallean -y --site-name=DurableDrupalDistro --account-name=admin --account-pass=admin --account-mail=dddadmin@awebfactory.com.ar --site-mail=durabledrupal@awebfactory.com.ar --db-url=mysql://ddd:dddpw22@localhost/ddd
You are about to DROP all tables in your 'ddd' database. Do you want to continue? (y/n): y
No tables to drop.                                                   [ok]
Starting Drupal installation. This takes a few seconds ...           [ok]
WD php: Warning: Invalid argument supplied for foreach() in          [warning]
_features_restore() (line 966 of
/home/drupallean/durable-drupal-distro/sites/all/modules/contrib/features/features.module).
Installation complete.  User name: admin  User password: admin       [ok]
~~~~~~~~

This is one time that the command-line is way quicker and more convenient than interactive mode!

### Test

We need to test that it is installed and running correctly before we make any changes.

We can now visit http://durable-drupal-distro.awebfactory.net/user, log in, and verify at http://durable-drupal-distro.awebfactory.net/admin/config/system/site-information that site is enabled with the following configuration as per the above drush site-install command parameters:

* Site name: DurableDrupalDistro
* E-mail address: durabledrupal@awebfactory.com.ar

and then at http://durable-drupal-distro.awebfactory.net/user/1/edit that

* Username: admin
* E-mail address: dddadmin@awebfactory.com.ar

while the database settings are verified both by the mysql info in sites/default/settings.php and by the fact that the site is operating.

Finally,

~~~~~~~~
$ drush status
 Drupal version                  :  7.34
 Site URI                        :  http://default
 Database driver                 :  mysql
 Database username               :  ddd
 Database name                   :  ddd
 Database                        :  Connected
 Drupal bootstrap                :  Successful
 Drupal user                     :  Anonymous
 Default theme                   :  drupallean
 Administration theme            :  seven
 PHP executable                  :  /usr/bin/php
 PHP configuration               :  /etc/php5/cli/php.ini
 PHP OS                          :  Linux
 Drush version                   :  6.2.0
 Drush configuration             :
 Drush alias files               :
 Drupal root                     :  /home/drupallean/durable-drupal-distro
 Site path                       :  sites/default
 File directory path             :  sites/default/files
 Temporary file directory path   :  /tmp
~~~~~~~~

### Update core and contrib

with drush

### Make any other changes

add linkit and picture

### Zap and reinstall to test

We need to test before commiting

### Commit distro without state

### Push to repo

### Tag and push tags
