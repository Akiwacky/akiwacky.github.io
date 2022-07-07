---
layout: page
title: Projects
permalink: projects
---

<div>
  {% for project in site.data.projects %}
    <div class="py-1">
      <h3><a href="{{project.url}}">{{ project.title}}</a></h3>
       <p class="text-gray-500 pb-0.5">{{project.bio}}</p>
      <div class="text-sm text-gray-400">{{project.date | date: "%B %-d, %Y"}}</div>
    </div>
  <div class="inline-flex items-center px-2.5 py-0.5 rounded-full text-xs font-medium bg-indigo-100 text-indigo-800">
     <a class="!no-underline">{{project.type}}</a>
  </div>
  {% endfor %}
</div>
