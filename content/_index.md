---
title: Home
sidebar:
  social: true
  entries:
    - title: Hacker On-Boarding
      url: "#intro"
      is_primary: true
    - title: Framing the project
      url: "#framing-the-project"
    - title: Choosing a solution
      url: "#choosing-a-solution"
      is_primary: false
    - title: Solutions
      url: "#solutions"
      is_primary: false
sections:
  - type: intro
    template: intro
    title: Hacker On-Boarding
    subtitle: We've created this site to provide information to help get your team off
      to a quicker start during dsmHack. Here you will find suggestions on various technology
      stacks that you can consider when building solutions for your nonprofit and some
      recommended best practices.
    section_id: intro
    background_style: style1
    actions: []
    component: intro.html
  - type: section
    template: section
    title: Framing the project
    subtitle: "The success of your project largely depends on understanding your nonprofit's true problem.
        Before you crack open your IDE and dive into the code, take some time to glean important insights
        up front, so that you can be more efficient with your time during the hack. Here are some tips for
        interviewing your nonprofit, forming a problem statement, mapping their story, and prioritizing work."
    section_id: framing-the-project
    background_style: style2
    actions:
      - label: Learn More
        url: /project-framing/
    component: section.html
  - type: features
    template: features
    title: Choosing a solution
    subtitle: 'Your team is welcome to choose any technology that you feel is best to
      help your nonprofit so please don''t feel you have to limit your team to the content
      of this site.  Just make sure to consider the following when choosing a solution:'
    section_id: choosing-a-solution
    background_style: style3
    features_list:
    - title: How much will it cost?
      text: Many of us work for business that are able to spend a lot of money on technology
        solutions.  The same is not usually true for nonprofit organizations.  Make
        sure you understand how much your nonprofit can afford and choose a solution
        that will stay within their budget.
      icon: fa-usd
    - title: How secure is it?
      text: Once your nonprofit leaves dsmHack they will likely be on their own to
        support and maintain the solution you build for them.  Many of our nonprofits
        do not have much experience with information security so making sure that you
        deliver them a solution that is secure and will stay secure for months and years
        after dsmHack is very important.
      icon: fa-lock
    - title: What is the learning curve?
      text: Your team likely consists of some very talented technology professionals
        who are capable of building some impressive custom solutions.  However, your
        nonprofits are not technology professionals.  They are going to be willing to
        learn a bit but definitely don't have time / desire to become experts in software
        engineering.  Make sure your solution fits their knowledge level and remember,
        part of your job at dsmHack is to train them.
      icon: fa-book
    - title: Can it be done in 48 hours?
      text: I'm sure you all have big ideas and we all appreciate your enthusiasm.  Just
        remember that at dsmHack time is not on your side.  You only have 48 hours (less
        if you manage to get some sleep) to design, implement, and test your solution
        as well as create documentation and train your nonprofit on how to use it.  So
        just make sure whatever you choose is doable in that small time window.
      icon: fa-clock-o
    component: features.html
  - type: spotlights
    template: spotlights
    title: Spotlights Section
    section_id: solutions
    background_style: style2
    component: spotlights.html
menu:
  main:
    name: Home
    weight: 1
layout: home
---
