---
# Leave the homepage title empty to use the site title
title: 'Yara Sleiman'
date: 2022-10-24
type: landing

sections:
  - block: hero
    content:
      title: Yara Sleiman
      text: Political Science Researcher at the London School of Economics
      primary_action:
        text: View Publications
        url: /publication/
        icon: download
  - block: biography
    id: about
    content:
      title: About me
      username: admin
  - block: collection
    id: papers 
    content:
      title: Recent Publications
      subtitle: ''
      text: ''
      count: 5
      filters:
        folders:
          - publication
        author: ""
        category: ""
        tag: ""
        exclude_featured: false
      archive:
        enable: true
        text: View All Publications
        link: publication/
    design:
      columns: '2'
      view: citation
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
  - block: contact
    id: contact
    content:
      title: Contact
      email: y.sleiman@lse.ac.uk
      address:
        street: Houghton Street
        city: London
        postcode: 'WC2A 2AE'
        country: United Kingdom
        country_code: UK
      directions: The London School of Economics and Political Science, Department of Government
      autolink: true
    design:
      columns: '2'
---
---
