---
# An instance of the Contact widget.
# Documentation: https://sourcethemes.com/academic/docs/page-builder/
widget: contact

# This file represents a page section.
headless: true

# Order that this section appears on the page.
weight: 130

title: Contact
subtitle:

content:
  # Automatically link email and phone or display as text?
  autolink: true
  
  # Email form provider
  form:
    provider: netlify
    netlify:
      # Enable CAPTCHA challenge to reduce spam?
      captcha: true
  
design:
  columns: '2'
---


** Contact page don't contain a body, just the front matter above.
See form.html in the layouts folder.

Formspree requires a (free) account and new form to be set up. The link is made on the final published url in the field: Restrict to Domain. It is possible to register up to 2 emails free and you can select which one you want the forms to go to within Formspree in the Settings tab.
**
