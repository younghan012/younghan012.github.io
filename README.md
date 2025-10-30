---
layout: default
title: Home
---

<style>
/* --- Simple CSS tabs (works without JS) --- */
.tabs { margin-top: 1rem; }
.tabs input { position: absolute; opacity: 0; }
.tabs .tab-label {
  display: inline-block; padding: .5rem 1rem; margin-right: .25rem;
  border: 1px solid #e1e4e8; border-bottom: 0; border-radius: 6px 6px 0 0;
  cursor: pointer; background: #f6f8fa; font-weight: 600;
}
.tabs .tab-label:hover { background: #eef1f4; }
.tabs .tab-content {
  display: none; border: 1px solid #e1e4e8; border-radius: 0 6px 6px 6px;
  padding: 1rem; background: #fff;
}
/* show content when its radio is checked */
#tab-edu:checked ~ #content-edu,
#tab-pub:checked ~ #content-pub,
#tab-teach:checked ~ #content-teach { display: block; }
/* active tab look */
#tab-edu:checked + label,
#tab-pub:checked + label,
#tab-teach:checked + label { background: #fff; border-bottom-color: #fff; }
</style>

# Youngjin Han

<div class="tabs">
  <!-- Education -->
  <input type="radio" name="tabs" id="tab-edu" checked>
  <label class="tab-label" for="tab-edu">Education</label>

  <!-- Publications -->
  <input type="radio" name="tabs" id="tab-pub">
  <label class="tab-label" for="tab-pub">Publications</label>

  <!-- Teaching -->
  <input type="radio" name="tabs" id="tab-teach">
  <label class="tab-label" for="tab-teach">Teaching</label>

  <!-- Content panes -->
  <div class="tab-content" id="content-edu">
    <h3>Education</h3>
    <ul>
      <li>Ph.D. Candidate, Your University (2021–present)</li>
      <li>M.S., Your University (2019)</li>
      <li>B.S., Your University (2017)</li>
    </ul>
  </div>

  <div class="tab-content" id="content-pub">
    <h3>Publications</h3>
    <ul>
      <li><strong>Paper Title</strong>, Conference/Journal, 2025. <a href="#">pdf</a></li>
      <li>Another Paper, 2024. <a href="#">arXiv</a></li>
    </ul>
  </div>

  <div class="tab-content" id="content-teach">
    <h3>Teaching</h3>
    <ul>
      <li>Instructor/TA, Course ABC (Fall 2024)</li>
      <li>TA, Course XYZ (Spring 2023)</li>
    </ul>
  </div>
</div>
