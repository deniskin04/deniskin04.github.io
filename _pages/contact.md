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
  .form-container { max-width: 100% }
  .form-container input { position: relative; top: 0; left: 0; width: 100%; height: 20px; padding: 0 ; }
  .form-container textarea { position: relative; top: 0; left: 0; width: 100%; height: 80px; padding: 0; }
</style>
<form action="https://formspree.io/f/mvgqjddl" method="POST">
  <label for="name">Your name</label>
  <input id="name" name="name" type="text" required>

  <label for="email">Your email</label>
  <input id="email" name="email" type="email" required>

  <label for="message">Message</label>
  <textarea id="message" name="message" rows="6" required></textarea>

  <!-- honeypot (spam trap) -->
  <input type="text" name="website" style="display:none" tabindex="-1" autocomplete="off">

  <!-- optional: subject for notifications -->
  <input type="hidden" name="_subject" value="New message from your website">

  <button type="submit" class="btn btn-primary">Send</button>
</form>

<p style="font-size:0.9rem;opacity:0.8;margin-top:1rem">
Thanks for getting in touch!
</p>