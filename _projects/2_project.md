---
layout: page
title: Author Analytics Dashboard
description: Freelance UX research and data product for self-published authors on LitNet.ru — turning fragmented performance data into decisions authors can actually act on.
img: assets/img/litnet_mainview.png
importance: 2
category: research
---

**Client:** Self-published online authors on LitNet.ru (20M+ combined views)  
**Role:** Researcher and data product designer  
**Methods:** User interviews, dashboard design, data pipeline, Chrome extension development

---

## The Problem

Authors on LitNet.ru — a large Russian-language self-publishing platform — had access to raw performance data (reads, ratings, comments, engagement) but it was fragmented and hard to interpret. There was no way to see trends across books, compare engagement over time, or figure out what was actually driving audience behavior.

The goal was to build something that surfaces patterns and helps authors make smarter decisions about publishing cadence, content focus, and ad spend — without drowning them in raw numbers.

---

## Research Process

### Phase 1: User Interviews

Started with in-depth interviews with authors to understand how they currently used performance data, what decisions they were actually trying to make, and where the gaps were.

Key themes that came up:
- No easy way to assess how many books to have active at once
- Comment sentiment was a meaningful signal that wasn't being tracked anywhere
- Authors wanted near real-time feedback, not periodic manual exports
- Hard to tell which books were worth putting ad spend behind

### Phase 2: Dashboard Design and Iteration

Built a data pipeline that aggregated and cleaned messy comment and engagement data, then designed a dashboard around the decisions authors were actually making:

- **Publication timeline (Gantt-style):** book activity across time, color-coded by engagement volume
- **Comment activity tracking:** 7-day and 30-day rolling averages alongside book open counts
- **Sentiment scoring:** tracks whether reader reactions are trending positive or negative

Iterated on the design through weekly feedback sessions with authors throughout the build.

<div class="row mt-4 justify-content-center">
    <div class="col-sm-10 mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/litnet_mainview.png" title="LitNet dashboard main view" class="img-fluid rounded z-depth-1" %}
        <div class="caption">Main dashboard view: publication timeline (Gantt) and comment engagement metrics</div>
    </div>
</div>

### Phase 3: Chrome Extension

A recurring friction point from the interviews was how painful it was to export data from LitNet manually. Built a Chrome extension ("Litnet Stats Collector") that lets authors fetch their full statistics in one click and download as JSON for direct upload to the dashboard.

This removed the main data-access bottleneck and made more frequent, up-to-date analysis possible.

---

## Impact

Author-reported outcomes from the dashboard:

- Identified **comment volume and sentiment** as the most actionable success metrics (previously not tracked at all)
- Helped authors figure out the **optimal number of concurrent active books**, which improved both output and work-life balance
- Gave a clear signal for which books were worth **digital ad spend**
- UX interview recommendations contributed to a **13% improvement in ad conversion**

---

## Key Takeaway

The most useful signal — comment sentiment — was already sitting in the data, just never aggregated. The research here was mostly about listening carefully to what decisions authors were actually trying to make, then building backward from that.
