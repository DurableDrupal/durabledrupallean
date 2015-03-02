# Appendix 2. Overcoming Choice Panic. What frameworks should we use? {#appendix-02}

At the onset of any project, the question inevitably arises: what frameworks should we use? 

We are be putting Choice Panic behind us and making a firm decision on the CMS framework we'll be using for our content-centric projects. First we'll place all our doubts right on the table for all to see: Should we be using Drupal for this project? really? is Drupal secure after 7.32? What about Backdrop? What about Drupal 8? Should we use that? Then we sift through the options, and choose the best one as our initial hypothesis. In making that decision we'll base ourselves on our current backlog of projects and on the information we actually have to go on right now. And that can change quickly, so we are not married to any framework, we simply want the best tools to get the job done. We'll explore that particular choice and the characteristics that make it the most versatile and dynamic option open to us. We want to be comfortable with the decision, and have the whole team all on the same page.

Now, also, above and beyond the framework, we are adopting a process which bases itself brutally on what we need and what our clients need, and which abandons vested vendor lock-in of any kind. We can't be married to any one set of frameworks any more. So the framework we select must be able to fit into our adopted, evolving and tailored process at a time when the industry is exploding with change and opportunities.

At the same time, we bear in mind that this is not a one-off question, but one which must be addressed periodically. The thing is, it must be addressed in order to allow you to work in a context of confidence that you are using the best tools for the job, instead of always having that question lurking in the back of your mind.

## "Building from Scratch" or not? Frameworks or not? {#building-from-scratch}

By starting from scratch what is usually meant is not actually starting with a blank page, but rather the use of light-weight frameworks and libraries over larger CMS frameworks. Light-weight frameworks might give you more freedom and flexibility and may be easier to start using, whereas larger frameworks offer a lot of built-in off-the-shelf functionality together with a large, easy to extend eco-system of plug-ins and add-ons. And using them often constitutes being part of a relatively large community of builders and users, offering possibilities for helping and being helped as well as for networking of many kinds.

### Starting from Scratch: Pros

Many developers are attracted towards smaller, light-weight libraries and components because they feel they will be dealing with less complexity, and will be able to be more creative and to "break new ground". They also feel they will not be stuck with a monolithic system and faced with the task of "turning off" a great deal of the built-in functionality not required for many projects, which is something not always easy to do. 

* You are building on top of shiny new technology
* Experimentation with new technologies and frameworks is not only fun but necessary in order to know what the options are.
* When a project is all about things that have never been done before, a completely straight-up ground-breaking disruptive [Blue Ocean](http://en.wikipedia.org/wiki/Blue_Ocean_Strategy) effort, it only makes sense to find a best-fit candidate architecture which doesn't complicate things with its extra baggage and lowest common denominator features which won't bring anything to the table or may even be a nuisance.

### Starting from Scratch: Cons

* If your are developing a content-centric project with many use cases that coincide with the larger CMS frameworks, then it really does not make any sense to reinvent the wheel. Countless features will have to be re-created: authentication and authorization (think: access rights for users and groups), forms management, database management, separation of concerns between business logic, data and the presentation layer, etc. It's a long list. 
* The larger CMS frameworks are constantly monitored for security threats and constantly offer security updates when threats emerge. So much so that to some (superficial) eyes the sheer number of security fixes seems to constitute evidence of their being more likely to come under attack. But experience shows this nothing could be further from the truth. One-off apps will need to dedicate considerable time and resources towards security issues on many levels.
* Starting from scratch may need a larger team, with more specialists compared to using a CMS framework.
* It is futile, for many use cases, to attempt to replace the work of whole communities across several years with a small team.
* You will have a harder time finding replacement team than you would if the project were being implemented with a large, well-known and highly adopted CMS framework like WordPress or Drupal, or Sitepoint.

D> Note: In this author's opinion, the learning curve necessary to acquire the skills required for the development of a modern website or web application tends to actually be the same, no matter whether you "start from scratch" or decide to use a large CMS framework. Even though learning a large CMS framework like Drupal, for example, may take several months in order to be productive, the same is equally true when it comes to getting up to speed with other frameworks. In the case of Drupal you may spend a lot of time learning "how things are done". But if you go the other route, you will be learning "how things are done" in a whole series of smaller frameworks; while needing to find out "how to do things" quite a bit more than you would have to in the former case. So, starting from scratch may take even longer. I would say it's six of one and half a dozen of the other. Furthermore, much of what "learning Drupal" is often said to entail actually includes things proper to the web application domain itself, such as server provisioning, e-commerce, email management, maintenance, testing frameworks, and methods of deployment, etc. So this isn't a pro or a con, again, in this author's opinion and experience.

D> "Frameworks don't scale!" Well, this is simply just not true. The Emmys, Weather.com, and many other examples abound. Of course, it's going to call for a lot of work to get a framework to scale. It's not the kind of work you expect to be doing when you signed up for a CMS framework either: Load balancers, Content Delivery Networks, HTTP and Database optimizations, accelerators, are just the start. Bud did you seriously think you were going to avoid all that just by using a lighter framework? Actually, it's all the same work. So this isn't a pro or con either.

In summary, reusability is an important principle and goal in software development, and for good reason. It is often summed up in the phrase "standing on the shoulders of giants". By observing this principle, one brings a necessary quota of zen modesty to the table and professionalizes ones activity. By admitting that existing CMS solutions have been perfected over time by their surrounding community of creators and users, and have honed issues such as security, functionality, ease of use, and many other fronts, developers gain power and productivity. There are CMS solutions for many different architectures and programming languages, and the best ones are fully customizable.

The reckless "hero" go-it-alone approach to software development, on the other hand, is often disguised improvisation, and a recipe for failure.

## Proprietary or not? Open-source or not?

Once the choice of framework has been made for a given project or series of projects, it must then be decided to go either with a proprietary or an open source solution.

On this subject, let's first take a look at the title of a fairly recent article: ["Open Source vs. Proprietary Software: There is No Clear Winner"[(http://www.cmswire.com/cms/information-management/open-source-vs-proprietary-software-there-is-no-clear-winner-021752.php#null). This might inflame the hearts and minds of many of us who have unquestionably supported open source over the years. But it's time to coldly ask ourselves: which has better code, and what's the low-down about true cost to market?

The article itself begins by asking why anyone would want to ever use anything but Open Source Software: "It’s free (or almost free); it’s built by passionate communities of developers; you can “look under the hood”; and there’s no vendor lock-in. Add to that, that the rate of innovation is supposed to be faster." And the short answer is that after a certain point of complexity is reached, it ceases to be true: it's no longer free even if there is no actual price tag on it, since the cost of (professional) use is much higher; it's increasingly built by company employees rather than a broad based passionate community; the rate of innovation ceases to be fast; and a kind of vendor lock-in arises out of the sheer scale becoming necessary for development, deployment and maintenance.

* According to Software development testing leader [Coverity](http://www.coverity.com), defect densities are practically identical. Where the [number of lines of code](http://www.ohloh.net) exceed 1 million, proprietary quality is better. The reason seems to be that not all open source projects have the budget to deal with the infrastructure required by the added complexity. Interestingly enough [Drupal has 970,000](http://www.ohloh.net/p?ref=homepage&q=drupal), just under the limit.
* "The true value in open source is the open, collaborative community of like-minded professionals who come together to crowd-source ideas and build great things" (Kevin Cochrane, Alfresco). But proprietary software vendors have huge community support to, as is undeniably the case with [Sharepoint Saturday's](http://www.spsevents.org). They have the "speakers", the "sponsors" and the T-shirts!
* In fact, there is a growing tendency within all open source frameworks for the number of very key core contributors to form part of an inner circle. In this way, the gap is closing between the relatively small number of "employee" committers on a proprietary project, on the one hand, and the ever-decreasing number of core committers on open source projects that grow in complexity. 
* Cost to market actually converges in both cases also, even though of course results may vary: Proprietary solutions charge an up-front and/or licensing price, but Open Source frameworks require considerable development, training and administratation costs to accomplish what the former does out-of-the-box.

D> In this author's opinion technical support and infrastructre service levels may be obtained for both kinds of frameworks; and there are more and more consultants, agencies and companies with an enormously high level of domain knowledge for either kind of framework also. These areas cannot really be considered to be an advantage for only proprietary frameworks.

Rather than the choice being between Proprietary and Open Source, it is more about the project's real needs. "Paying developers to massively customise an open source CMS may end up costing you more than paying for a proprietary solution that more closely meets your requirements. On the flip side, paying license fees for an ill-suited proprietary solution doesn't make any sense either."  (See [Choosing Between an Open Source or Proprietary Website CMS](http://www.netxtra.net/insights/choosing-between-an-open-source-or-proprietary-website-cms/)).

## [WordPress](https://wordpress.org/) or not?

The stark fact here is that, from a CMS framework perspective, WordPress is less than Drupal, unless what you really want is an elegant industry-standard blog. While Drupal is a superset of WordPress, and one may migrate to Drupal comfortably without expecting to miss any features, the opposite is certainly not the case. 

Unless your use cases coincide with the functionality offered by WordPress, in which case you still have a choice to make, the following points point consistently in Drupal's favor:

* It's when you contemplate porting a Drupal web application to a WordPress website that the latter's shortcomings really stand out.
* Despite [Easy Post Types](https://wordpress.org/plugins/easy-post-types/) Drupal wins hands down in terms of being able to create business objects with content types, having support for all kinds of field types, plus field collections and other features.
* Users are just another entity in Drupal and can use the same patterns that any old business object (taxonomy term, content type item, user, etc.) uses.
* Separation of concerns between the dynamic data model, the semantic HTML containing the dynamic content of the business object data model, and the styling to be applied to this basic unadorned un-styled HTML (that's called semantic HTML) is very well observed in Drupal, but badly supported in Wordpress, which means parrallel team development work is greatly impaired.
* WordPress has nothing like Drupal's Views: a complete and intuitive SQL Query Generator that's so intuitive most users don't realize it's an SQL Query Generator. It's really easy to list your stuff in all kinds of different ways.
* Rules module: built in support for UI based business rules, plus the ability to roll your own in code.
* Huge amount of very rich extensions (Drupal modules):
  * Complete layout and theming development system alternatives
    * [Page Manager and Panels](https://www.drupal.org/project/panels) (either with [Panopoly](https://www.drupal.org/project/panopoly) or do it yourself (as we do in our [DurableDrupalDistro](https://github.com/victorkane/drupal-lean))
    * [Display Suite](https://www.drupal.org/project/ds)
    * [Context module](https://www.drupal.org/project/context)
  * Workflow modules
    * [Workbench](https://www.drupal.org/project/workbench)
    * [Workflow](https://www.drupal.org/project/workflow)
* Everything in code alternatives allow us to break the back of configuration in the database, and help our teamwork. 

## [Drupal](https://drupal.org/) or not?

Drupal, together with its particularly rich eco-system, is a perfect fit for many content-centric projects because it offers such a complete set of solutions to the problems and challenges historically facing developers of dynamic websites and web application. Its features cover the whole cycle of design, development, deployment and maintenance:

* Dynamic website and web application framework with complete separation of concerns between business objects, data persistence, business logic and presentation.
* Social web platform
* Prototyping tool for Business objects and data modeling, data viewing, layout and styling
* Modern web design templating system allowing for further separation for concerns within the presentation layer, of semantic content, layout and styling.
* Built in and customizable Content Management and Editorial Workflow System 
* Well-documented and established tools and procedures make for full compatibility with best practices on development process and devops levels.

Drupal sits under the 1 million lines of code limit, which would indicate that it is a project whose quality has greatly benefited over the years from having been developed by a diverse and large international
community. Since the code is open source, it has been  available to all to freely criticize, modify (or at least propose patches in issue queues), and discuss. It is in fact one of the most sophisticated CMS frameworks around, whether open source or proprietary, capable of supporting the development of large-scale content-centric web application projects. 

Many of the benefits of Drupal stood out in the previous section when it was compared to WordPress. But there's more.

### Community and Intelligence

Drupal has a truly international community, with a huge amount of communication, sharing of responsibility and participation of all kinds going on across borders at all times. Each year there are two international conferences (DrupalCon), one in Europe and one in the US. 2015 will see the first [DrupalCon Latin America](https://latinamerica2015.drupal.org/). In addition, Drupaleros in many cities all over the world hold annual Drupal camps, some having a long and rich history such as the Bay Area's [BADCamp](https://badcamp.net/). There are [many additional ways](https://www.drupal.org/community), online and off, that interaction takes place in the community. It can be said in many ways that technical expertise is part and parcel of the Drupal culture, as is the case in many open source communities.

And since the Drupal community is not based solely in a single country, but rather all over the world, the approach tends to be more cosmopolitan and "out of the box", with people looking for deep and permanent solutions and not simply quick fixes based on a "common sense" empirical ways of thinking. That's why even though Drupal could have been written off quickly with the advent of Server side java script and a bevy of front-end frameworks (as of course it could be one day), or perhaps by new offerings from other programming environments and architectures, a huge critical mass of intelligence has forged Drupal into something truly modern. This promises years of competitive mojo: separation of concerns with adaptive back and front-ends, straightforward integration with multi-tiered and distributed components, REST interfaces both for stand-alone servers and clients.

### Easily extensible

#### Modules

Since highly talented people have always been attracted to the community, solutions have constantly emerged keeping those leveraging Drupal for their content-centric projects on the technological vanguard with minimal effort. In a rich, mature eco-system, there is, literally, "a module for everything", and not just those with sexy features, but also those promising integration with all major players in the modern web app universe. Today, for example, with no coding you can whip up a fully functional social network based platform with a back-end API, with node.js based chat and activity stream, and with a totally mobile first responsive theme to top it off in literally hours.

#### Distributions

In addition many first-class Drupal installation profiles ("distros") are available. These off-the-shelf domain-specific customizable solutions tailor Drupal to specific project needs. Some of the best examples:

* [CiviCRM Starter Kit](https://www.drupal.org/project/civicrm_starterkit): a web-based, open source, CRM geared toward meeting the needs of non-profit and civic-sector organizations. The starter kit integrates CiviCRM with Drupal.

* [DKAN[(https://github.com/NuCivic/dkan): a Drupal-based open data platform with a full suite of cataloging, publishing and visualization features that allows governments, nonprofits and universities to easily publish data to the public.

* [Commerce Kickstart](https://www.drupal.org/project/commerce_kickstart): a software distribution for sites of any size that provides all the power and flexibility of Drupal Commerce, combined with components that accelerate creation and launch of an online store.

* [Open Academy](https://www.drupal.org/project/openacademy): a web publishing solution for higher education.

* [OpenAid](https://www.drupal.org/project/openaid): a turnkey website platform designed to help cause-driven organizations create cost-effective program-focused websites quickly.

* [Open Atrium 2](https://www.drupal.org/project/openatrium): open source collaboration software that enables organizations to securely connect their teams, projects, and knowledge.

* [OpenIdeaL](https://www.drupal.org/project/idea): an idea management system, for both public and commercial sectors. It is a powerful tool to analyze public opinion regarding products/services and identify trends.

* [Open Outreach](https://www.drupal.org/project/openoutreach): a Drupal distribution written to provide grassroots, activist, and nonprofit groups with the web tools they need for effective public engagement.

* [OpenPublic](https://www.drupal.org/project/openpublic): provides a content management system specially designed for open government goals, without compromising accessibility, security or usability.

* [Panopoly](https://www.drupal.org/project/panopoly): an off-the-shelf responsively themed, Panels based distribution designed to be a base framework upon which to build other Drupal distributions (among others, OpenAcademy and Open Atrium), but will also work for general site building.

* [Plato Típico](https://www.drupal.org/project/plato_tipico): This is a a preconfigured distro with multi-language support for English & Spanish. Already comes with most of the necessary modules which will save you lots of time and research.

* [Pushtape](https://www.drupal.org/project/pushtape): Build better music websites with Pushtape, a Drupal distribution for musicians. Manage your music discography, create news updates, upload photos, post upcoming shows and more.

Many may be installed with a single click on the [Pantheon](https://www.getpantheon.com/) platform, for example.

#### Themes

The Drupal theme system is everything that the superficial and outmoded industry standard "template" concept is not. Themes allow for the meticulous separation of semantic data and business logic, on the one hand, from the layout, styling and formatting of the presentation layer, on the other. Characteristic of Drupal, they provide compelling alternatives for design-level customization.

### Recognizable, standard architecture

If you build it with Drupal, automatically an increasing number of readily available Drupal development talent is available all over the world who will recognize how you web app is built, and be able to provide maintenance or further development as you wish. Compared to the effort required for a developer to comprehend the anatomy of a one-off custom application, that is a decided advantage and greatly enhances the lifetime value of your project.

### An abundance of Drupal-friendly deployment options

Depending on the scale of what you are deploying, there are a host (pardon) of infrastructure alternatives: From shared hosting (yes, it's gotten better), to VPS and cloud PaaS, including the Pantheon platform mentioned above. It's getting easier and easier for Drupal based web applications to enjoy smooth delivery and maintenance.

So much internationally active talent, so much engineering, so much quality! Drupal excels as a CMS and Web Application Framework.

## Drupal 8 or not?

### Benefits of Drupal 8 {#appendix-02-d8-benefits}

> "Drupal 8 will set a new standard for ease of use, while offering countless new ways to tailor and deploy your content to the Web. Easily customize data structures, listings, and pages, and take advantage of new capabilities for displaying data on mobile devices, building APIs, and adapting to multilingual needs.

> "With a leaner and meaner core, easier migration process from earlier versions, in-place content editing tools and loads more power for modules and themes thanks to a modern Object Oriented Programming (OOP) approach on the backend, there is something for everyone to love in Drupal 8. When will it be released? [See the FAQ](https://drupal.org/drupal-8.0/faq)."
> > [drupal.org on Drupal 8](https://www.drupal.org/drupal-8.0)

Larry Garfield, in his presentation at DrupalCon Latin America 2015 in Bogotá summed up the benefits of Drupal 8 in startling fashion (see [video](https://www.youtube.com/watch?v=-lLILaIZr44) and [slides](http://www.palantir.net/presentations/dcbogota2015-drupal-and-us/#/2/1) when he explained that not only is Drupal 8 a new generation PHP Platform, but that far from what we have been led to expect, namely that it will only be useful for experienced developers and for large companies with huge resources, in actual fact it can do much more than any other CMS framework, for everyone, right off-the-shelf even for plain old site-building right in core without any configuration:

| Drupal 7 | Drupal 8 |
|----------|----------|
|PHP4 architecture|PHP 5.4 architecture|
|Everything is a page|Everything is a (different kind of) response|
|All home grown|Embrace other communities and tools|
|A good start for a CMS|Build real-world sites right away just with core|

* Benefits for site builders **for everyone, out of the box**: Build real sites with what comes in core, without any configuration
  * More fields in core (Entity Reference, Date, Link, Email, Telephone) with the Field API (rich data model just with core)
  * Views API and UI in core (saves 6 months in terms of being able to use Drupal 8 after initial RC release, compared to having had to wait for views when Drupal 7 was released, without Views in core)
    * Admin uses views, much more customizable (VBO in core!)
    * Content modeling, editing, assembly, delivery out of the box
    * Content delivery
  * Configuration management based on versionable YAML text files; the configuration is no longer mixed with content in the database
    * Much better solution for dev -> testing -> production workflow and deployment
    * Everyone, large and small, has the right to have access to configuration management tools
    * Real Configuration API
    * Config import/export built in
    * Modules can include default config
  * Translation (of interface, content AND configuration!) has been completely revamped, compacted, improved and better integrated in core
* Benefits for content editors
  * Rich editing experience (in core: WYSIWYG editor, editing in place, more usable forms; works without configuration)
  * Back to site button (instead of overlay :) )
  * Accessibility WAI-ARIA, keyboard control, voice control with Drupal Announce API so that reportedly a sight-impaired person may edit in place. Best accessibilityt there is. All built in and automatic.
  * New text-based help system (including context-sensitive help)
* For themers
  * Out with IE6-8
    * Module for IE8 if you need it
  * HTML5 + CSS3
  * Everything responsive out of the box (including menus and toolbars)
  * HTML5 Forms which also work on mobile!
  * [Twig](https://www.drupal.org/theme-guide/8/twig) template engine.
    * Instead of PHP required for templates, designers only need knowledge of TWIG
  * 25% fewer divs
* Benefits for coders (under the hood)
  * Modern version of PHP 5.4, re-visioning how Drupal uses a modern language.
  	* Interface-driven development
  	* Loose coupling
  	* "Hack core without hacking core"; fewer Drupalisms
  	* No more Not Invented Here; now Proudly Invented Elsewhere
  	  * Symfony2 components (HttpFoundation, HttpKernel, DependencyInjection, EventDispatcher, Routing, Serializer, Validator, Yaml)
  	  * Symfony CMF (Content Management Framework, co-authored by the Symfony, Easy CMS and Drupal communities)
  	  * Zend Feed (including Atom, and with greatly reduced dependencies)
  	  * Doctrine Annotations
  	  * Guzzle (best Http client in PHP)
  	  * EasyRDF
  	  * Twig
  * Plugins: same pattern used all over
  * Unified entity API, used all over
  * Unit tests with PHPUnit
  * RESTful pipeline
  * Drupal has gotten off the island, meaning that general development experience in many PHP projects transfer to Drupal 8 and multiple platforms
  * Drupal Console built on Symfony Console for scaffolding and code generation, instrospection and profiling

In addition:

* Block is just another entity
* The Drupal 7 context module is now in core

It is no accident that the keynote, an example of excellent community leadership ("Drupal is a platform for the independent. For everyone. By all of us. Drupal 8 is going to kick-ass") caused huge excitement, and set the record straight for Drupal 8.
  	
However interesting Drupal 8 may appear to be, though, it cannot be used at the present time for production website or web applications.

### When will Drupal 8 be able to be used for production ready projects? {#appendix-02-when-d8-prod} 
>"Drupal 8 is currently in development and is not yet ready for production use."
> > *[drupal.org](https://www.drupal.org/documentation/version-info)*

### Drupal 8 will be ready for non-trivial site building sometime in 2016
[Drupal Planet](https://www.drupal.org/planet) consensus seems to indicate that Drupal 8 will probably not have a production ready release until around mid-to-late-2015, and that another 6-12 months will have to go by before:

* The offering becomes stable and complete.
* Most third party modules and distributions get ported to Drupal 8, if at all, or replaced (or, as we have emphasized, might already be in core, so it's not the same as with previous major Drupal releases).
* A critical mass of Drupal developers become profficient in Drupal 8 development and it becomes cost-effective to equip a team with available developers.

You will have to calculate true development costs yourself since third-party based functionality you take for granted today (and may or may not use depending on your current project) may not be available.

The best criteria for being able to start production ready sites was given in the above-cited presentation by Larry Garfield (@crell), in which he pointed out that the single most important block to actually using Drupal 8 for projects is the current absence of an automatic upgrade path for beta to beta releases. And it's best to wait until a release candidate is out or about to be out.

## Straight up [Symfony](http://symfony.com/) or not?

Why not just go with Symfony then and just skip the Drupal Drama? We owe it to ourselves to consider this alternative coldly and professionally. Our question has to be, just what are the merits of website and web application development just going with Symfony?

But using Symfony "instead" of Drupal is roughly equivalent to [Starting from Scratch](#building-from-scratch): Either you replace Drupal yourself individually with your own development resources (pretty difficult) or you replace it with another framework. 

Symfony being a PHP based framework is going to be an advantage for some and a disadvantage for others. On the one hand it leverages the skills you have gained with Drupal or other frameworks without having to learn a new language or actually set of front-end and back-end languages (javascript, go, java/scala, ruby, etc.). On the other, some developers who are looking to grow beyond PHP, or [feel it is limited in some way](http://eev.ee/blog/2012/04/09/php-a-fractal-of-bad-design/), if they are going to go with a lighter framework would prefer to go with one of the non-PHP alternatives.

## [Backdrop](https://backdropcms.org/) or not?

Backdrop was forked from Drupal as a reaction against Drupal 8 for the following reasons:

The [Roadmap for Backdrop 1.0](https://backdropcms.org/roadmap) lists the following:

* Configuration Management System
* Built-in Content Listing Generator
* Revamped Layout System
* Improved Performance
* Improved Mobile Support
* Reduced Theme System Complexity

How well will these be implemented?

Will it attain community critical mass?

Will it think out a proper workflow (i.e. be a solution for devs as well as end users)?
The most important Backdrop feature is workflow with everything in code. D8 already has their workflow. What's Backdrop's? Difficulties in getting onto Pantheon for example, show workflow not thought out.
For example, export and import of config from one system to another is easy in the GUI. But what if I want to automate that with ansible as part of a deployment scheme? In my opinion, we would want code+db+files+config, we don't want config to be mixed either with code for all sites (since it is specific to one) ... we don't want you to have to push files or push database to live!!!!!!! 

The exciting news recently has been the release of Backdrop 1.0.0. We'll come back to this (see how it matures) in the Migrations volume (next) in the DurableDrupal series (or there might be a Backdrop CMS workbook companion to this book).

We'll fork Backdrop CMS, practice using it, then make a push request or else at the very least raise an issue concerning workflow blockers when we write Vol. 2 (Migrations) for the DurableDrupal series.

## Drupal 7 or not?

### State of Drupal 7

Drupal 7 is mature, full of add-ons, modules, distros, and quality base themes many of which offer an out-of-the-box responsive front-end. There is a huge community of skilled designers and developers thoroughly experienced in the release, so building a team is much more accessible than most other options. And Drupal 7 will still be officially supported for another three years or so, and then probably for some time after that, at least informally (as has been the case with other releases). 

It's available right now as an option for including much of the hotness of Drupal 8 without the learning curve. Given the complete panorama we have been examining, Drupal 7 is a high-quality, low-cost alternative that should definitely be considered first, and only discarded if there exist unusual requirements on a given project.

Now, this very maturity and rich flexibility, plus the breadth and experience gained in the community with Drupal 7 gives us an exciting perspective: the makings of a Drupal LTS distro we can build on now and maintain for years to come. 

### Why a distribution?

To understand the importance of basing ourselves on a Drupal distribution, or installation profile, let's review the procedures that would normally be followed in the context of firing up a new project:

1. Prepare a development instance on a LAMP stack somewhere with a database and a runnable document root
1. Run the standard Drupal 7 install profile on that development instance
1. Get rid of the irritating cruft
1. Decide which responsive layout systems to include (Drupal core blocks and [Context](https://www.drupal.org/project/context), [Panels](https://www.drupal.org/project/panels), [Display Suite](https://www.drupal.org/project/displaysuite))
1. Create a sub-theme from the base theme of your choice (i.e. [AdaptiveTheme](https://www.drupal.org/project/adaptivetheme), [Zen](https://www.drupal.org/project/zen), [Omega](https://www.drupal.org/project/omega), just to name three) compatible with your layout systems
1. Install the third-party contrib modules without which you cannot build a site and which our experience has told us are good solid building blocks ([80/20 rule](http://en.wikipedia.org/wiki/Pareto_principle#In_software))

Then, when you want to fire up a separate staging instance for acceptance testing with the client, you:

1. Prepare a development instance on a LAMP stack somewhere with a database and a runnable document root
1. Copy over the code (Drupal) and the files (assets)
1. Dump the dev database and populate the staging database
1. Edit settings.php
1. Clear cache :)

A lot of the bother can be solved, it's true, using the famous "everything in code" paradigm, especially for continuous delivery to staging from dev, and we'll see how that's done later:

1. Create a repo on GitHub/Bitbucket or similar
1. Export the current state into versionable text files (we'll see how a bit later on) and push to the repo 
1. Clone this master dev site from the repo to staging
1. Clear cache :)

**What if we could automate this process, eliminating the need to execute these steps manually, over and over again, every time we fire up a new project?** 

What would we need to be able to do that?

Answer: An on-going in-house Drupal distribution. Together with a lean agile process (skip ahead), a repo-based everything-in-code development discipline (skip ahead), and a [DevOps](http://en.wikipedia.org/wiki/DevOps) automation platform for provisioning, deployment, and orchestration (like [Puppet](http://puppetlabs.com/), [Chef](https://www.chef.io/chef/), [Ansible](http://www.ansible.com/home): skip ahead).


That's why a distribution must form the heart of our process.

## Presenting [DurableDrupalDistro](https://github.com/victorkane/durable-drupal-distro) with Lean process

This book will allow us to tool up a website and web app factory process on the solid basis of forking, using, and repeating our best practices as we re-use the DurableDrupalDistro. 

Whether we are talking about working on our local workstation or laptop, on a PaaS (Platform as a Service) like Pantheon or Platform.sh, or whether we are going to be using a VPS or cloud instance of our own, the secret is to automate DevOps on the basis of our very own Drupal distribution. This all-important in-house Drupal distribution, will evolve with us from project to project and become part of an organization's library of distributions as teams get formed around new projects. It will be branched and tailored (with the diff merged back in, wholly or partially, in order to benefit future projects). And it will be the stepping stone to migrations to other Drupal releases, to Symfony, or any other future framework the future may hold for us. We will be able to build a development process of best practices around it, and set up our own veritable web factory.

Fork it, tailor it, maintain it, branch and release it over all your projects!

Evolve it, build a team process around it and grow it into the future!

In this chapter, given a project we need to get started on, a dynamic website for a neighborhood non-profit that runs programs for youth in the community, we've laid all our options face-up on the table, we've taken a decision on what's best to use right now. We reviewed starting from scratch, proprietary and open-source frameworks, WordPress and Drupal, Drupal 8, Backdrop CMS, Drupal 7, and, given Drupal 7, the use of a distribution, the DurableDrupalDistro, as a starting point upon which to build.

In the next chapter we'll take the DurableDrupalDistro and run with it and build our project. 
