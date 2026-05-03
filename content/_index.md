---
title: 'Home'
date: 2023-10-24
type: home
---
  - block: biography
    content:
      username: me
      # Show a call-to-action button under your biography? (optional)
      button:
        text: Download Résumé
        url: uploads/resume.pdf
    design:
      show_status: false
      spacing:
        padding: ['0', '0', '6rem', '0']
      banner:
        # Upload your cover image to the `assets/media/` folder and reference it here
        filename: kalen-emsley-Bkci_8qcdvQ-unsplash.jpg
      biography:
        # Customize the style of your biography text
        style: 'text-align: justify; font-size: 0.8em;'
      # Avatar customization
      avatar:
        size: large # Options: small (150px), medium (200px, default), large (320px), xl (400px), xxl (500px)
        shape: rounded # Options: circle (default), square, rounded
  - block: experience
    content:
      username: me
    design:
      # Hugo date format
      date_format: 'January 2006'
      # Education or Experience section first?
      is_education_first: false
  - block: portfolio
    content:
      title: Side Projects
      filters:
        folders:
          - projects/side-projects
      buttons:
        - name: All
          tag: '*'
        - name: Technology 1
          tag: technology1
        - name: Technology 2
          tag: technology2
    design:
      columns: '1'
      view: masonry
      flip_alt_rows: false
  - block: portfolio
    content:
      title: Work Projects
      subtitle: Generic descriptions of projects highlighting business impact and value
      filters:
        folders:
          - projects/work-projects
      buttons:
        - name: All
          tag: '*'
        - name: Business Impact
          tag: business-impact
    design:
      columns: '1'
      view: masonry
      flip_alt_rows: false
  - block: skills
    content:
      title: Skills & Hobbies
      username: me
  - block: awards
    content:
      title: Awards
      username: me
  - block: languages
    content:
      title: Languages
      username: me
---
