---
layout: post
title: "Update"
author: Turtle
categories: site-update
---

Hello, It's Turtle, so today i've been trying to get this site ready for use as quickly as possible. So far I've added a page called [about]({{site.url}}/about)
I am currently trying to get this website setup for the members of my group so that they can post to this as well.

Currently, the members that we have will be at the bottom of this page.

<ul>
{% for member in site.data.members %}
  <li>
    {{ member.name }}
    <a href="https://github.com/{{ member.github }}">GitHub</a>  
    <a href="http://github.com/{{ member.twitter }}">Twitter</a>
  </li>
{% endfor %}
</ul>