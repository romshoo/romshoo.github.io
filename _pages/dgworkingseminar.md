---
layout: page
permalink: /dgworkingseminar/
title: Waterloo Differential Geometry Working Seminar
nav_title: dgws
description: 
nav: true
nav_order: 5
---

<style>
  .dgws-tabs {
    display: flex;
    gap: 0.6rem;
    align-items: center;
    flex-wrap: wrap;
    margin: 1rem 0 1.5rem;
  }

  .dgws-tabs-label {
    font-weight: 700;
    margin-right: 0.25rem;
  }

  .dgws-tab {
    background: transparent;
    border: 1px solid #ced4da;
    border-radius: 0.35rem;
    color: inherit;
    cursor: pointer;
    font: inherit;
    padding: 0.35rem 0.75rem;
  }

  .dgws-tab.active {
    background: #343a40;
    border-color: #343a40;
    color: #fff;
  }

  .dgws-entry {
    margin: 1.4rem 0;
  }

  .dgws-entry-date {
    font-weight: 700;
    margin-bottom: 0.35rem;
  }

  .dgws-semester-panel[hidden] {
    display: none;
  }
</style>

<div class="dgws-tabs" aria-label="Semesters">
  <span class="dgws-tabs-label">Semester:</span>
  <button class="dgws-tab active" type="button" aria-selected="true" data-semester="fall-2026">Fall 2026</button>
  <button class="dgws-tab" type="button" aria-selected="false" data-semester="winter-2027">Winter 2027</button>
  <button class="dgws-tab" type="button" aria-selected="false" data-semester="spring-2027">Spring 2027</button>
  <a class="dgws-tab" href="/~fromshoo/assets/html/DG%20Website/workingseminar_home.html">Previous schedules</a>
</div>

<div class="dgws-semester-panel" data-semester-panel="fall-2026">
<p> 🍂 Tuesdays 2:30 to 4:00 p.m. in MC 5417 🍂</p>
<div class="dgws-entry">
  <div class="dgws-entry-date">Sep 15, 2026</div>
  <div><strong>Speaker: </strong> Spiro Karigiannis</div>
  <div><strong>Title:  </strong> Organizational Meeting</div>
  <div><strong>Abstract: </strong> We will plan the speakers for the rest of the semester. </div>
</div>
<div class="dgws-entry">
  <div class="dgws-entry-date">Sep 22, 2026</div>
  <div><strong>Speaker:</strong> Viktor Majewski</div>
  <div><strong>Title:</strong> TBA</div>
  <div><strong>Abstract:</strong> TBA</div>
</div>
<div class="dgws-entry">
  <div class="dgws-entry-date">Sep 29, 2026</div>
  <div><strong>Speaker:</strong> Facundo Camano</div>
  <div><strong>Title:</strong> TBA</div>
  <div><strong>Abstract:</strong> TBA</div>
</div>
<div class="dgws-entry">
  <div class="dgws-entry-date">Oct 6, 2026</div>
  <div><strong>Speaker:</strong> Paul Cusson</div>
  <div><strong>Title:</strong> TBA</div>
  <div><strong>Abstract:</strong> TBA</div>
</div>
<div class="dgws-entry">
  <div class="dgws-entry-date">Oct 13, 2026</div>
  <div><strong>Reading week</strong> </div>
  
</div>
<div class="dgws-entry">
  <div class="dgws-entry-date">Oct 20, 2026</div>
  <div><strong>Speaker:</strong> Spencer Kelly</div>
  <div><strong>Title:</strong> TBA</div>
  <div><strong>Abstract:</strong> TBA</div>
</div>
<div class="dgws-entry">
  <div class="dgws-entry-date">Oct 27, 2026</div>
  <div><strong>Speaker:</strong> Faisal Romshoo </div>
  <div><strong>Title:</strong> TBA</div>
  <div><strong>Abstract:</strong> TBA</div>
</div>
<div class="dgws-entry">
  <div class="dgws-entry-date">Nov 3, 2026</div>
  <div><strong>Speaker:</strong> Benoit Charbonneau</div>
  <div><strong>Title:</strong> TBA</div>
  <div><strong>Abstract:</strong> TBA</div>
</div>
<div class="dgws-entry">
  <div class="dgws-entry-date">Nov 10, 2026</div>
  <div><strong>Speaker:</strong> Francisco Villacis</div>
  <div><strong>Title:</strong> TBA</div>
  <div><strong>Abstract:</strong> TBA</div>
</div>
<div class="dgws-entry">
  <div class="dgws-entry-date">Nov 17, 2026</div>
  <div><strong>Speaker:</strong> Jacques Van Wyk </div>
  <div><strong>Title:</strong> TBA</div>
  <div><strong>Abstract:</strong> TBA</div>
</div>
<div class="dgws-entry">
  <div class="dgws-entry-date">Nov 24, 2026</div>
  <div><strong>Speaker:</strong> Faisal Romshoo </div>
  <div><strong>Title:</strong> TBA</div>
  <div><strong>Abstract:</strong> TBA</div>
</div>
<div class="dgws-entry">
  <div class="dgws-entry-date">Dec 1, 2026</div>
  <div><strong>Speaker:</strong> Danial Ghamari</div>
  <div><strong>Title:</strong> TBA</div>
  <div><strong>Abstract:</strong> TBA</div>
</div>
<div class="dgws-entry">
  <div class="dgws-entry-date">Dec 8, 2026</div>
  <div><strong>Speaker:</strong> Spencer Kelly</div>
  <div><strong>Title:</strong> TBA</div>
  <div><strong>Abstract:</strong> TBA</div>
</div>
<div class="dgws-entry">
  <div class="dgws-entry-date">Dec 15, 2026</div>
  <div><strong>Speaker:</strong> Danial Ghamari</div>
  <div><strong>Title:</strong> TBA</div>
  <div><strong>Abstract:</strong> TBA</div>
</div>
</div>

<div class="dgws-semester-panel" data-semester-panel="winter-2027" hidden>
  <p>TBD</p>
</div>

<div class="dgws-semester-panel" data-semester-panel="spring-2027" hidden>
  <p>TBD</p>
</div>

<script>
  document.querySelectorAll(".dgws-tab[data-semester]").forEach((tab) => {
    tab.addEventListener("click", () => {
      const semester = tab.dataset.semester;

      document.querySelectorAll(".dgws-tab[data-semester]").forEach((item) => {
        const isActive = item === tab;
        item.classList.toggle("active", isActive);
        item.setAttribute("aria-selected", isActive);
      });

      document.querySelectorAll(".dgws-semester-panel").forEach((panel) => {
        panel.hidden = panel.dataset.semesterPanel !== semester;
      });
    });
  });
</script>
