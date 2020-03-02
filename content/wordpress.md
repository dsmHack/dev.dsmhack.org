---
title: WordPress
home_spotlights:
  enabled: true
  weight: 1
  excerpt: WordPress is one of the most well-known and popular content management
    system (CMS) solutions available.  It is built on PHP and MySQL and has thousands
    of templates and plug-ins available to extend its functionality.
  home_img:
    path: images/wordpress.jpg
    data_position: center center
    url: "#"
layout: page
---

[WordPress](https://wordpress.org/) has been a popular choice among dsmHack teams for many years. There are over 55,000
plug-ins available to extend its functionality.

## Past projects

These are some examples of past dsmHack projects which were built using WordPress:

* [Jolly Holiday Lights](https://www.jollyholidaylights.org/) - (2019)
* [Iowa Radio Reading](https://www.iowaradioreading.org/) - (2019)
* [Community Support Advocates](https://teamcsa.org/) - (2019)
* [RoofTop Foundation](http://rooftopfoundation.org/) - (2017)
* [Help-A-Heart](https://help-a-heart.org/) - (2015)

## Is WordPress right for your project?

Here are some of the pros and cons we've learned over the years at dsmHack to help you decide if WordPress is the right
choice for your project.

### Pros

* **Easy for end users to update content**

  This is probably one of the biggest selling points for WordPress.  It comes with a fully featured user interface for
  managing your site and it's content out-of-the-box.  That being said, don't think this means there is no learning
  curve.  If you are just building simple pages and blog post then it should be pretty simple to learn but as soon as
  you start using plugins for more complicated content things become a bit less user-friendly.

* **Plug-ins**

  At the time this was written there were well over 55,000 plugins available for WordPress.  If there is something you
  want to do on your site chances are there is a plugin for it.  Of course, with that many plugins then that means there
  will likely be more than one plugin to solve your problem.  So, sometimes it can be difficult to deciding which plugin
  you should choose.

* **Themes**

  Similar to plugins there are an endless number of themes available for WordPress.

### Cons

* **Maintenance**

  While a WordPress site is really easy to get up and running, maintaining it can be an entirely different story.
  WordPress has automatic updates built-in for the platform, themes, and plug-ins.  However, if you've made any
  customizations to your theme then updating it will likely overwrite all of your customizations.  In addition, many
  times plug-ins are not compatible with all versions of WordPress so you can find yourself in a situation where you
  want to update WordPress but doing so would result in a plug-in no longer working.  This can be very frustrating to
  manage and is something most of our nonprofits will have a hard time understanding.  The main thing you can do to
  mitigate this is limit your plug-in usage to only mainstream and well supported plug-ins and either don't customize
  your theme or if you do customize it make a copy of it and customize the copy.

* **Vulnerability**

  Being the most popular CMS has it's downsides and one of the biggest is that it means WordPress always has a target on
  it's back.  WordPress is notorious for having vulnerability issues and this is why the previous point above about
  maintenance is so important.  You need to keep WordPress up-to-date to make sure you have the latest security patches.
  It's also very important you have strong passwords and preferably two factor authentication on the admin site.  Also,
  it's recommended to turn off the ability to post comments on every page unless the nonprofit needs that feature.

* **Performance**

  A fresh install of WordPress will have seemingly no issues with performance. However, as soon as you start adding in a
  theme and several plugins, more often than not you will start to see a slow down.

* **Collaborative Development**

  One of the biggest challenges we see at dsmHack is how difficult it can be to collaborate within WordPress. It's
  common to see issues with multiple people editing the same thing at the same time and end up overriding each other's
  work.  There are plenty of strategies available to help mitigate these issues though and we talk a bit more about that
  in the *Development Process* section below.

## Getting started

If you decide WordPress is the right choice for your team's project then you will have several other decisions to make.
Before you can really get started you will need to decide on hosting, a theme, and what your development process will
look like.

### Hosting

First decision you will need to make is where you will host the WordPress site.  The two primary types of hosting
available are *managed hosts* and *unmanaged hosts*:

1. **Managed Host** - A managed host handles most of the details of deploying and managing a WordPress site for you so
   that you can focus on building out the design and content of the site.  These hosts may provide automatic backups,
   upgrades, caching, SEO support, enhanced security, among other services.  Overall, a managed host will be more
   reliable than an unmanaged host but downside to a managed host is that you tend to have less flexibility in what you
   can do with WordPress.  For instance, many managed hosts limit which plugins you can install. Some others do not
   allow you to access the database that backs your website.  You'll need to weigh the pros and cons of these benefits
   and limitations with your team to make the right choice for your nonprofit.  Some examples of popular managed hosts
   include but are not limited to [WordPress.com](https://wordpress.com), [WP Engine](https://wpengine.com/),
   [Kinsta](https://kinsta.com/), or [Flywheel](https://getflywheel.com/).
2. **Unmanaged Hosts** - An unmanaged host will give you the most flexibility and often times they will allow you to
   deploy more than just WordPress sites. You will normally setup your site using
   [cPanel](https://hostingfacts.com/beginners-guide-to-cpanel/) or a similar web based configuration tool. After the
   WordPress site and database have been created the host won't usually have much to do with anything else.  You are
   likely on your own to figure out all the things mentioned above that the managed hosts would do for you.  As stated
   above, unmanaged hosts just carry some more risk with them because all that responsibility is on you. If you are only
   choosing to use an unmanaged host because you want to use a plugin that the managed hosts don't allow, just make sure
   your team discusses whether or not that plugin is worth it.  Some examples of popular unmanaged hosts include but are
   not limited to [Siteground](https://www.siteground.com/), [Dreamhost](https://www.dreamhost.com/),
   [Bluehost](https://www.bluehost.com), or [GoDaddy](https://godaddy.com).

For more information about various hosting options you may find this write-up from [CodeinWP](https://codeinwp.com)
which they titled [Best WordPress Hosting](https://www.codeinwp.com/blog/best-wordpress-hosting/). Please just note that
we are not officially recommending any specific host or endorsing any recommendation from CodeinWP. Ultimately, this
decision falls on your team to make.

### Theme

It is very common to overhear dsmHack teams having spirited debates over which WordPress theme to choose. There is lot
to consider past just the superficial.  It's very rare that a team is good with using a theme exactly how it comes
out-of-the-box so you'll need to understand which pieces you will want to change and whether or not the theme provides
you the ability to customize the theme through configurations. Generally, free themes do not provide many customization
capabilities so you may also need to consider paying for a premium theme that gives you those possibilities.

### Development Process

At dsmHack we usually see a couple of different approaches to WordPress development.

#### Production development

The first is what we will call "just doing it all in production".  This is exactly how it sounds.  You stand-up the
website on your production domain and everyone just gets in there and starts making changes.  This has some benefits. In
particular, the biggest benefit for a 48-hour hack is that you are already in production from the start so there is no
worry that you still need to get past that hurdle. Of course, there are the obvious downsides as well. The risk is much
greater that you will make a change that breaks something and won't be able to revert back. You really should avoid this
option if the site is already live.  If you are using a managed hosting solution then this might be your only choice but
many of them provide staging environments so you can make changes and test them before pushing it to the production site
(another advantage of managed hosts).

#### Local development

The other approach is to run a local version of WordPress for development.  The advantage of running WordPress locally
is that you remove any risk of causing impact to your other team members and the production site.  You can try out new
plugins and themes without worry. Also, you won't have to worry about any network issues since everything is local. The
downside is that you'll need to come up with a deployment strategy to actually move everything from your local site to
the production site and you'll need to deal with merging your changes with changes from your team.

There is no one and only way to handle this so you will need to figure the best process that works with your team. To
get the conversation going here are some examples:

* [WordPress: Using Docker
  Compose](https://fabianlee.org/2019/03/17/wordpress-cloning-your-wordpress-site-locally-using-docker-compose/)
* [WordPress Deployment Workflow: How I Roll](https://carriedils.com/wordpress-deployment-workflow/)
* [No More Cowboy Coding: Improving Your WordPress
  Workflow](https://premium.wpmudev.org/blog/improve-wordpress-development-workflow-local-server/)
* [Deploying WordPress](https://spinupwp.com/wordpress-deployment-workflow-preparing/)
* [Development Workflow Best Practices](https://wpengine.com/support/development-workflow-best-practices/)
* [WordPress Local Development For
  Beginners](https://www.smashingmagazine.com/2018/04/wordpress-local-development-beginners-setup-deployment/)
* [Search Google](https://www.google.com/search?q=wordpress+local+development+deployment)

The best thing to do is to figure all of this out before you start building the site.  Too many times, we've seen teams
who have their website all built out 2 hours before final presentations but it's all on one person's laptop and they are
scrambling to figure out how to get it deployed.  Having this figured out on the first day of the hack will set your
mind at ease and allow you to deploy multiple times as you build the site out so that you know you will be ready to go
for the final presentation.  Just make sure you also manage your time effectively.  You only have 48 hours so if you are
still figuring out development and deployment strategies on Friday morning then you are going to fall behind.
