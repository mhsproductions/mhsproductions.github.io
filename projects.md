---
layout: default
title: MHSProductions
active_tab: projects
---
<!-- This file pulls from projects.yaml -->

### Homework

<table class="table table-striped">
  <thead>
    <tr>
      <th>Name</th>
      <th>Date Built</th>
      <th>Languages</th>
    </tr>
  </thead>

  <tbody>
    {% for project in site.data.projects %}
    <tr style="text-align: left">
        <td><a href = "projects/{{ project.link }}">{{ project.name }}</a></td>
        <td>{{ project.date }}</td>
        <td>{{ project.languages }}</td>
    </tr>
    {% endfor %}
  </tbody>
</table>
