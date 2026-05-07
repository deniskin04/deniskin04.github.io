---
layout: page
title: Author Analytics Dashboard
description: Freelance UX research and data product for self-published authors on LitNet.ru — turning fragmented performance data into actionable decisions.
img:
importance: 2
category: research
---

**Client:** Self-published online authors on LitNet.ru (20M+ combined views)  
**Role:** Researcher + data product designer  
**Methods:** User interviews · Dashboard design · Data pipeline · Chrome extension development

---

## The Problem

Authors on LitNet.ru — a large Russian-language self-publishing platform — had access to raw performance data (reads, ratings, comments, engagement), but it was fragmented and hard to interpret. There was no way to see trends, compare books, or identify what was actually driving audience behavior.

**Goal:** surface patterns that help authors make smarter decisions about publishing cadence, content focus, and ad spend — without drowning them in raw numbers.

---

## Research Process

### Phase 1 — User Interviews

Conducted in-depth interviews with authors to uncover how they currently used performance data, what decisions they were trying to make, and where the gaps were.

Key themes that emerged:
- Authors struggled to identify which books warranted promotional investment
- There was no easy way to assess optimal number of concurrent active books
- Comment sentiment was a meaningful signal that wasn't being tracked at all
- Authors wanted near real-time feedback, not periodic manual exports

### Phase 2 — Dashboard Design & Iteration

Built a data pipeline that aggregated and cleaned messy comment and engagement data, then designed a dashboard with metrics and visualizations directly tied to author decision-making:

- **Publication timeline (Gantt-style):** visualizes book activity across time, color-coded by engagement volume
- **Comment activity tracking:** 7-day and 30-day rolling averages alongside book open counts
- **Sentiment scoring:** surfaces whether reader reactions are trending positive or negative

Iterated on design based on weekly feedback sessions with authors throughout the build.

### Phase 3 — Chrome Extension

Based on ongoing author interviews, a recurring friction point emerged: exporting data from LitNet was manual and tedious. Built a **Google Chrome extension** ("Litnet Stats Collector") that allows authors to fetch their complete statistics in one click and download as JSON for direct upload to the dashboard.

This removed the data-access bottleneck and enabled more frequent, up-to-date analysis.

---

## Impact

Author-reported outcomes from the dashboard:

- Identified **comment volume and sentiment** as the most actionable success metrics (previously unmeasured)
- Enabled authors to pinpoint **optimal number of concurrent active books** — improving both output quality and work-life balance
- Provided a clear signal for which books warranted **digital ad spend**
- Recommendations from UX interviews contributed to a **13% improvement in ad conversion**

---

## Key Takeaway

The insight that mattered most wasn't a new metric — it was discovering that the most useful signal (comment sentiment) was already there in the data, just never aggregated. Good research here meant listening carefully to what decisions authors were actually trying to make, then designing backward from that.
