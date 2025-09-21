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
    id: papers 
    content:
      title: Selected papers
      text: |-
        {{% callout note %}}
        Quickly discover relevant content by [filtering papers](./publication/).
        {{% /callout %}}
      filters:
        folders:
          - publication
        exclude_featured: true
    design:
      columns: '2'
      view: citation
  - block: collection
    id: wp
    content: 
      title: Working Papers
      text: |-
        {{% callout note %}}
        Quickly discover relevant content by [filtering working papers](./wp/).
        {{% /callout %}}
      filters:
        folders:
          - wp
        exclude_featured: true
    design:
      columns: '2'
      view: citation      
  - block: portfolio
    id: projects
    content:
      title: Projects
      filters:
        folders:
          - project
      # Default filter index (e.g. 0 corresponds to the first `filter_button` instance below).
      default_button_index: 0
      # Filter toolbar (optional).
      # Add or remove as many filters (`filter_button` instances) as you like.
      # To show all items, set `tag` to "*".
      # To filter by a specific tag, set `tag` to an existing tag name.
      # To remove the toolbar, delete the entire `filter_button` block.
      buttons:
        - name: All
          tag: '*'
        - name: Public Policy
          tag: Econ
        - name: Development
          tag: Dev
        - name: Other
          tag: Other
    design:
      # Choose how many columns the section has. Valid values: '1' or '2'.
      columns: '1'
      view: showcase
      # For Showcase view, flip alternate rows?
      flip_alt_rows: false
  - block: collection
    id: teaching
    content:
     title: Teaching
     filters:
      folders:
        - teaching
     design:
       columns: '2'
       view: compact
  # - block: tag_cloud
  #   content:
  #     title: Popular Topics
  #   design:
  #     columns: '2'
  - block: contact
    id: contact
    content:
      title: Contact
      subtitle:
      text: |-
        You can contact me or book an appoinment at:
      # Contact (add or remove contact options as necessary)
      email: y.sleiman@qmul.ac.uk
      appointment_url: 'https://calendly.com/g-melios'
      address:
        street: 
        city: 
        postcode: 
        country: 
        country_code: 
      directions: 
      office_hours:
      # Choose a map provider in `params.yaml` to show a map from these coordinates
      # contact_links:
      #   - icon: twitter
      #     icon_pack: fab
      #     name: DM Me
      #     link: 'https://twitter.com/GeorgeMelios'
      # Automatically link email and phone or display as text?
      design:
      columns: '2'
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
