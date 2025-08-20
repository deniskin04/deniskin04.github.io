---
layout: page
permalink: /contact/
title: Contact
description: Use the form below to contact me.
nav: true
nav_order: 4
---

## Send a message

<style>
  /* Vertical, stacked form */
  .form-container{
    max-width: 640px;
    margin: 0 auto;
    display: grid;
    grid-template-columns: 1fr;
    gap: 1rem;
  }
  .form-container label{
    display: block;
    font-weight: 600;
    margin-bottom: .25rem;
  }
  .form-container input,
  .form-container textarea{
    width: 100%;
    box-sizing: border-box;
    padding: .7rem .9rem;
    border: 1px solid var(--color-border, #e5e7eb);
    border-radius: .5rem;
    background: var(--color-bg, #fff);
  }
  .form-container button{ margin-top: .25rem; }

  /* If theme tries to lay out horizontally */
  .form-container{ flex-direction: column !important; align-items: stretch !important; }
</style>

<form class="form-container" action="https://formspree.io/f/mvgqjddl" method="POST">
  <label for="name">Your name</label>
  <input id="name" name="name" type="text" autocomplete="name" required>

  <label for="email">Your email</label>
  <input id="email" name="email" type="email" autocomplete="email" required>

  <label for="message">Message</label>
  <textarea id="message" name="message" rows="6" required></textarea>

  <!-- honeypot (spam trap) -->
  <input type="text" name="website" style="display:none" tabindex="-1" autocomplete="off">

  <!-- optional: email subject + redirect after submit -->
  <input type="hidden" name="_subject" value="New message from your website">
  <!-- <input type="hidden" name="_redirect" value="{{ '/contact/thanks/' | absolute_url }}"> -->

  <button type="submit" class="btn btn-primary">Send</button>
</form>