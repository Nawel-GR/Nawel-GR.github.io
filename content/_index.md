---
# Leave the homepage title empty to use the site title
title: ''
summary: ''
date: 2022-10-24
type: landing

sections:
  # Biography: photo moved to the left via assets/css/custom.css (no education here).
  - block: resume-biography
    id: about
    content:
      # Author profile to display — a slug in `data/authors/` (this site uses `me`)
      username: me
      text: ''
      button:
        text: Download CV
        url: uploads/resume.pdf
    design:
      # No gradient_mesh — let the clean Minimal theme background show through.
      avatar:
        size: medium # small | medium | large | xl | xxl
        shape: circle # circle | square | rounded
  # Styled Education + Experience (education first).
  - block: resume-experience
    id: experience
    content:
      username: me
    design:
      date_format: 'January 2006'
      is_education_first: true
  - block: portfolio
    id: projects
    content:
      title: Projects
      filters:
        folders:
          - projects
    design:
      columns: 2
      fallback_icon: code-bracket
  - block: collection
    id: publications
    content:
      title: Publications
      filters:
        folders:
          - publications
    design:
      view: citation
  - block: collection
    id: events
    content:
      title: Talks & Events
      filters:
        folders:
          - events
    design:
      view: card
  - block: contact-info
    id: contact
    content:
      title: Contact
      subtitle: Open to collaborations in ML, NLP and applied research.
      username: me
      email: nahuel.gomez@ug.uchile.cl
      social:
        - icon: brands/linkedin
          url: https://www.linkedin.com/in/nahuel-gomez-raguileo/
        - icon: brands/github
          url: https://github.com/Nawel-GR
      show_form: false
---
