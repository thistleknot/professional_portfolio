---
title: ''
summary: ''
date: 2026-05-03
type: landing

sections:
  - block: dev-hero
    id: hero
    content:
      username: me
      greeting: "Hi, I'm"
      show_status: false
      show_scroll_indicator: true
      typewriter:
        enable: true
        prefix: "I build"
        strings:
          - "production semantic AI systems"
          - "domain-specific RAG pipelines"
          - "agentic orchestration tooling"
          - "quantitative research workflows"
        type_speed: 65
        delete_speed: 40
        pause_time: 2400
      cta_buttons:
        - text: View Projects
          url: "#projects"
          icon: arrow-down
        - text: View Experience
          url: "#experience"
          icon: briefcase
    design:
      style: centered
      avatar_shape: rounded
      animations: true
      background:
        color:
          light: "#f5f7fa"
          dark: "#0f1419"
      spacing:
        padding: ["6rem", "0", "4rem", "0"]

  - block: portfolio
    id: projects
    content:
      title: "Selected Projects"
      subtitle: "Reasoning models, semantic retrieval, quantitative research, optimization, and technical media work."
      count: 0
      filters:
        folders:
          - projects
      buttons:
        - name: All
          tag: '*'
        - name: SOTA
          tag: sota
        - name: Quant
          tag: quantitative-finance
        - name: NLP
          tag: nlp
        - name: Music
          tag: music-production
      default_button_index: 0
    design:
      columns: 3
      fallback_icon: code-bracket
      background:
        color:
          light: "#ffffff"
          dark: "#0d1117"
      spacing:
        padding: ["4rem", "0", "4rem", "0"]

  - block: tech-stack
    id: skills
    content:
      title: "Technical Breadth"
      subtitle: "Applied across AI systems, infrastructure, research workflows, and media production."
      categories:
        - name: AI Systems
          items:
            - name: PyTorch
              icon: devicon/pytorch
            - name: Transformers
              icon: code-bracket
            - name: RAG / Semantic Retrieval
              icon: magnifying-glass
            - name: Knowledge Graphs
              icon: share
        - name: Data + Infrastructure
          items:
            - name: PostgreSQL / pgVector
              icon: devicon/postgresql
            - name: Docker
              icon: devicon/docker
            - name: Kubernetes
              icon: devicon/kubernetes
            - name: GitLab CI/CD
              icon: brands/gitlab
        - name: Research + Quant
          items:
            - name: Dask
              icon: circle-stack
            - name: Airflow
              icon: cloud
            - name: Time Series Forecasting
              icon: chart-bar
            - name: Portfolio Optimization
              icon: scale
        - name: Media + Signal
          items:
            - name: Music Embeddings
              icon: musical-note
            - name: FL Studio
              icon: musical-note
            - name: Interactive Visualization
              icon: sparkles
            - name: Audio Engineering
              icon: speaker-wave
    design:
      style: grid
      show_levels: false
      background:
        color:
          light: "#f8fafc"
          dark: "#080c12"
      spacing:
        padding: ["4rem", "0", "4rem", "0"]

  - block: experience
    id: experience
    content:
      username: me
    design:
      date_format: 'January 2006'
      is_education_first: false

  - block: cta-card
    content:
      title: "Open to the right ML / AI engineering opportunity"
      text: |-
        I work best where **semantic AI**, **production engineering**, and **research fluency** intersect.

        You can find more at [GitHub](https://github.com/thistleknot), [LinkedIn](https://linkedin.com/in/joshualaferriere), and [SoundCloud](https://soundcloud.com/user-344326160).
      button:
        text: "View GitHub"
        url: "https://github.com/thistleknot"
        new_tab: true
    design:
      card:
        css_class: 'bg-gradient-to-br from-slate-200 via-slate-100 to-blue-100 dark:from-slate-800 dark:via-slate-900 dark:to-slate-700'
        text_color: dark
      background:
        color:
          light: "#f8fafc"
          dark: "#080c12"
      spacing:
        padding: ["4rem", "0", "6rem", "0"]
---
