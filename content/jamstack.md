---
title: JAMStack
home_spotlights:
  enabled: true
  weight: 2
  excerpt: Fast and secure sites and apps delivered by pre-rendering files and serving
    them directly from a CDN, removing the requirement to manage or run web servers.
  home_img:
    path: images/pic02.jpg
    data_position: top center
    url: "#"
layout: page
---

The [JAMStack](https://jamstack.org) is strategy for building websites where all the pages are pre-rendered and served
directly from a CDN.  Pages are generated at build time by pulling in content from either flat files written with a
markup language or from a headless CMS and then applying that content against layout templates to generate HTML. A
JAMStack site is typically referred to as a *static site* since all the pages end up being static HTML files.  However,
this is not an entirely accurate description of a JAMStack site. A JAMStack site can still have very dynamic content but
rather than re-rendering HTML to provide that dynamic content the site instead uses JavaScript and APIs to bring in
dynamic content and only when that content must truly be dynamic. This combination of **J**avaScript, **A**PIs, and
**M**arkup is why we call them *JAMStack* sites.

## Past projects

These are some examples of past dsmHack projects which were built using JAMStack: '

* [Les Dames d'Escoffier](https://lesdamesdsm.org/) [{{< fa github >}}](https://github.com/dsmHack/2019-team-07) (2019)
* [dsmHack - Hacker On-Boarding](https://dev.dsmhack.org/) [{{< fa github
  >}}](https://github.com/dsmHack/dev.dsmhack.org) (2019)

## Is JAMStack right for your project?

There are several benefits to choosing a JAMStack solution vs a dynamic site like WordPress, but there are some
downsides as well.  Here are some pros and cons to consider:

### Pros

* **Performance**

  There are several reasons you will get better performance from a JAMStack site.  Since all the pages are generated at
  build time they can be deployed directly to a CDN rather than to a web server.  This also means that users are not
  waiting precious seconds for database queries to be ran and HTML to be generated because all of that was done at build
  time. You also get the benefit of simple scaling since most CDNs provide scaling in their services.

* **Security**

  The simpler infrastructure of a JAMStack site means there is no database or web server that can become compromised.
  Any APIs used by your site can be broken into micro-services and server-less functions to reduce attack areas.  You
  can also leverage expertise of third-party services.

* **Collaboration**

  Using a version control system like Git is a vital and natural part to building a JAMStack site.  This makes it very
  simple to collaborate with a team to build the site. Everyone can pull down the source code and generally have a
  development version of the site running with only a couple of commands.  If something gets broken, you can easily
  revert back to a previous version of the site without losing a sweat.  Also, depending on the build service you are
  using you can even have preview versions of your site created for each pull request so changes can be verified before
  they are deployed to production.  These are all features that feel very simple and out-of-box with JAMStack but are
  usually much more complicated with a dynamic solution like WordPress.

* **Flexibility**

  For a developer and designer, a JAMStack site allows a lot more flexibility to build and design the site the way they
  want and using the technologies they want.  A theme is more of a starting point that you are encouraged to customize
  to fit your needs.  It is also usually much simpler to create a theme from scratch than it is with a dynamic site like
  WordPress because themes are just simple template files.

### Cons

* **Overwhelming amount of choices**

  Sure, choice is a good thing.  But there are new solutions for building JAMStack sites popping up everyday and that
  can making choosing the right one very overwhelming.  You only have 48 hours at dsmHack so you can't spend much time
  looking at all the possible solutions.  To help with this, we offer some suggestions below to help you streamline your
  decision.

* **Learning Curve**

  In a lot of ways this con isn't really fair.  If you've never used WordPress before then the learning curve can be
  pretty steep there as well.  The difference here is that many people have experience with WordPress so it's probably
  easier to get support at this point.  That being said, WordPress and all of its plugins and themes can feel a lot
  like a black box at times which make the learning curve difficult when trying to customize your site.  Since JAMStack
  sites are basically all contained to flat files within a source repository it's much easier to dig in and figure out
  what is happening so in the long term it is easier to have a full understanding of how your site works.

## Getting started

Before you can begin building your site you will need to choose a static site generator, a headless CMS, a theme, and a
host.

### Static Site Generators

The static site generator (SSG) is a tool responsible for generating your site.  There are several to choose from and
while they all generally do the same thing they are definitely not all created equal.  The site,
[StaticGen.com](https://www.staticgen.com/), provides a summary of most of the known generators available.  It provides
several metrics to help you gauge the maturity and popularity of a generator like number of stars and number of issues
on Github. It also lets you filter by programming language and template language. In the end this is your teams decision
and it will drive all the next decisions you make. We recommend you consider the following:

* **Maturity and Popularity**

  Many of these projects haven't been around a long time so maturity is a little tough to determine but at least stay
  away from a generator that has only be around a month or two.  Popularity is also important because if you choose a
  generator no one else is using then it will be much harder to get help with it.  Just remember that many times the
  most popular solution isn't always the most mature because people always get excited about the new thing.

* **Languages**

  You definitely don't need to be familiar with the language that your static site generator is written in.  For
  example, this website is built using [Hugo](https://gohugo.io/) but we have no experience using the Go programming
  language it is written in.  The more important language is the template language that is used. It is common that you
  will want to either modify your theme's templates or add new templates so making sure it is a template language that
  either you already know or can learn easily is important. Again, while we don't have experience with building
  applications using Go, we've found writing Go templates for this website to be fairly simple.

* **Ease of use**

  This one is hard to determine without actually using the generator for a little bit but there are some things you can
  check on to help give you a good idea on it.  First, look at what is required to install it.  For Hugo, you just
  install a single binary.  For [Gatsby](https://www.gatsbyjs.org/Gatsby), you need to install NodeJS and NPM and then
  you just install Gatsby like any other NPM package.  Next check to see if there is some sort of a "quick start"
  documentation for the generator and read through it to determine how quick the process of just getting a simple site
  running will be. For example, you can find Hugo's quick start [here](https://gohugo.io/getting-started/quick-start/)
  and Gatsby's quick start [here](https://gatsbyjs.org/docs/quick-start/).

### Headless CMS

Whenever I mention the idea of using JAMStack for a dsmHack project I almost always get the same response. It
basically goes like this, "How do you expect nonprofits to know how to update markdown files and a Git repository?" This
usually is the result of someone only having experience using [Jekyll](https://jekyllrb.com/) with [Github
Pages](https://pages.github.com/) for a project that only ever required a developer be involved.  The truth is there are
several solutions for managing content of JAMStack sites that offer full featured user interfaces completed with WYSIWYG
editors. These solutions are referred to as a headless CMS.

The site, [headlessCMS.org](https://headlesscms.org/), provides a summary of most of the known headless CMS solutions
available. Similar to the StaticGen site mentioned above this site will allow you to quickly compare the popularity and
maturity of the headless CMS as well as filter on the type of CMS and their compatibility with various static site
generators.

There are two primary types of headless CMS solutions: Git-based and API driven.

* **Git-based**

  A Git-based CMS uses your projects Git repository as the storage solution for all the content.  It will typically keep
  several files that contain meta-data describing the structure of your content and then build its user interface using
  those files.  Some of these CMS solutions like [NetlifyCMS](https://www.netlifycms.org/) run entirely within your site
  and only use a third-party for authentication of users.  Others, like [Forestry](https://forestry.io/), host the entire
  admin user interface through their own site and just connect to your Git repository to make changes.  The biggest
  benefit of a Git-based CMS is that your entire site is all in the Git repository and versioned. If you ever decide to
  change to another CMS or the CMS you are currently using shuts down then you don't have any data to migrate because it
  already there in your repository and your site will continue to build the same way regardless.

* **API driven**

  An API driven CMS stores your content in a database and provides APIs for retrieving that content when your site is
  being built. The benefit of using an API driven CMS is that it is much simpler to create complex data models.  If you
  use a hosted API driven CMS solutions like [Contentful](https://www.contentful.com/) then management of the database
  and users is handled by the CMS provider which can make things pretty simple to setup.  You can also use an open
  source API driven CMS like [Strapi](https://strapi.io/) but you will then need to host the CMS and the database
  yourself on a service like AWS which will begin to complicate things.

### Theme

You'll need to choose a theme to start out.  Most of the static site generators have their own list of themes that are
available but there are also theme sites that allow you to search for themes across various site generators.  One of
those sites is [JAMStack Themes](https://jamstackthemes.dev/).  It gives you the ability to filter on various properties
of the theme and view a live demo of the theme.

### Hosting

There are several possibilities for hosting your static site but the most popular are [Github
Pages](https://pages.github.com/) and [Netlify](https://www.netlify.com/). While Github Pages is a great solution, the
feature set available from Netlify makes it our recommended pick based on these three features alone:

* **Automatic Build & Deployment**

  Github Pages offers automatic build & deployment but only for Jekyll based sites.  If you want to host sites built
  with other site generators on GitHub Pages you will need to also add a solution for building and deploying the site
  using something like [GitHub Actions](https://github.com/features/actions), [TravisCI](https://travis-ci.org/), or
  similar tool.  Netlify on the other hand has built-in support for building and deploying sites built with most of the
  [popular generators](https://docs.netlify.com/configure-builds/common-configurations/) and it's beta [build image
  selection](https://docs.netlify.com/configure-builds/get-started/#build-image-selection) support enables you to build
  with any generator you choose.

* **Deploy Previews**

  [Netlify deploy previews](https://docs.netlify.com/site-deploys/overview/#deploy-preview-controls) will build a
  preview of your site for all your pull requests so you can verify your changes before merging them.  This is a very
  powerful feature and really helps teams collaborate.

* **Serverless Functions**

  [Netlify Functions](https://www.netlify.com/products/functions/) allow you to write simple serverless functions
  powered by AWS Lambda.  This allows you to greatly extend the functionality available within your site without needing
  to involve any other server platform.
