---
layout: default
title: "People"
---

<div class="main-section-wrap">
  <div class="title-wrap">
    <h3>Director</h3>
  </div>
  <section class="people-grid">
  {% for person in site.data.people.director %}
    {% include people-item.html
      name=person.name
      role=person.role
      department=person.department
      school=person.school
      image=person.image
      link=person.link %}
  {% endfor %}
  </section>
</div>

<!-- #FIXME: For future post docs -->
<!-- <div class="main-section-wrap">
  <div class="title-wrap">
    <h3>Post Docs</h3>
  </div>
  <section class="people-grid">
  {% for person in site.data.people.current_postdoc %}
    {% include people-item.html
      name=person.name
      role=person.role
      department=person.department
      school=person.school
      image=person.image
      link=person.link %}
  {% endfor %}
  </section>
</div> -->

<div class="main-section-wrap">
  <div class="title-wrap">
    <h3>PhD Students</h3>
  </div>
  <section class="people-grid">
  {% for person in site.data.people.current_phd %}
    {% include people-item.html
      name=person.name
      role=person.role
      department=person.department
      school=person.school
      image=person.image
      link=person.link %}
  {% endfor %}
  </section>
</div>

<!-- #FIXME: For future master inters/students -->
<!-- <div class="main-section-wrap">
  <div class="title-wrap">
    <h3>Masters students</h3>
  </div>
  <section class="people-grid">
  {% for person in site.data.people.current_masters %}
    {% include people-item.html
      name=person.name
      role=person.role
      department=person.department
      school=person.school
      image=person.image
      link=person.link %}
  {% endfor %}
  </section>
</div> -->

<div class="main-section-wrap">
  <div class="title-wrap">
    <h3>Alumni</h3>
  </div>
  <div class="alumni-list-wrap">
    <ul class="people-list">
      {% for person in site.data.people.alumni %}
        {% if person.link %}
        <li><a href="{{person.link}}" target="_blank">{{person.name}}</a>, {{person.position}}</li>
        {% else %}
        <li><span class="name">{{person.name}}</span>, {{person.position}}</li>
        {% endif %}
      {% endfor %}
    </ul>
  </div>
</div>
