---
# Leave the homepage title empty to use the site title
title: 'Yara Sleiman'
date: 2022-10-24
type: landing

sections:
  - block: about.biography
    id: about
    content:
      title: About me
      # Choose a user profile to display (a folder name within `content/authors/`)
      username: admin
  # - block: experience
  #   content:
  #     title: Affiliations
  #     # Date format for experience
  #     #   Refer to https://docs.hugoblox.com/customization/#date-format
  #     date_format: Jan 2006
  #     # Experiences.
  #     #   Add/remove as many `experience` items below as you like.
  #     #   Required fields are `title`, `company`, and `date_start`.
  #     #   Leave `date_end` empty if it's your current employer.
  #     #   Begin multi-line descriptions with YAML's `|2-` multi-line prefix.
  #     items:
  #       - title: Research Officer
  #         company: London School of Economics and Political Science
  #         company_url: ''
  #         location: London
  #         date_start: '2021-10-01'
  #         date_end: ''
  #       - title: Senior Research Fellow (Hon)
  #         company: University College London
  #         company_url: ''
  #         location: London
  #         date_start: '2020-01-01'
  #         date_end: ''
  #   design:
  #     columns: '1'
  - block: collection
    id: research
    content:
      text: |-
        # Research {#research-heading}

        ### Publications
      filters:
        folders:
          - publication
        exclude_featured: true
    design:
      columns: '2'
      view: citation
      spacing:
        padding: ['3rem', '0', '0', '0']
  - block: collection
    id: research-rr
    content:
      text: |-
        ### Revise & Resubmit
      filters:
        folders:
          - rr
        exclude_featured: true
    design:
      columns: '2'
      view: citation
      spacing:
        padding: ['0', '0', '0', '0']
  - block: collection
    id: research-wp
    content:
      text: |-
        ### Working papers
      filters:
        folders:
          - wp
        exclude_featured: true
    design:
      columns: '2'
      view: citation
      spacing:
        padding: ['0', '0', '3rem', '0']
  - block: markdown
    id: teaching
    content:
      text: |-
        # Teaching {#teaching-heading}

        Seminar Leader, Queen Mary University of London

        - Quantitative Methods for Social Science Research
        - Political Analysis
        - Introduction to Political Science
        - Comparative Politics
    design:
      columns: '2'
  - block: markdown
    id: contact
    content:
      text: |-
        # Contact {#contact-heading}
    design:
      columns: '2'
      spacing:
        padding: ['3rem', '0', '0', '0']
  - block: contact
    id: contact-details
    content:
      text: |-
        You can contact me at:
      email: yarajsleiman@gmail.com
      appointment_url: ''
      address:
        street:
        city:
        postcode:
        country:
        country_code:
      directions:
      office_hours:
    design:
      columns: '2'
      spacing:
        padding: ['0', '0', '3rem', '0']
  # - block: collection
  #   id: posts
  #   content:
  #     title: Recent Posts
  #     subtitle: ''
  #     text: ''
  #     # Choose how many pages you would like to display (0 = all pages)
  #     count: 5
  #     # Filter on criteria
  #     filters:
  #       folders:
  #         - post
  #       author: ""
  #       category: ""
  #       tag: ""
  #       exclude_featured: false
  #       exclude_future: false
  #       exclude_past: false
  #       publication_type: ""
  #     # Choose how many pages you would like to offset by
  #     offset: 0
  #     # Page order: descending (desc) or ascending (asc) date.
  #     order: desc
  #   design:
  #     # Choose a layout view
  #     view: compact
  #     columns: '2'
---
