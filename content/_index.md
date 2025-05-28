---
# Leave the homepage title empty to use the site title
title:
date: 2023-06-27
type: landing

sections:
  - block: hero
    content:
      title: Hello and welcome
    #   image:
    #     filename: home-background.jpg
      # cta:
      #   label: '**Get Started**'
      #   url: https://wowchemy.com/templates/
      # cta_alt:
      #   label: Ask a question
      #   url: https://discord.gg/z8wNYzb
      # cta_note:
      #   label: >-
      #     <div style="text-shadow: none;"><a class="github-button" href="https://github.com/wowchemy/wowchemy-hugo-themes" data-icon="octicon-star" data-size="large" data-show-count="true" aria-label="Star">Star Wowchemy Website Builder</a></div><div style="text-shadow: none;"><a class="github-button" href="https://github.com/wowchemy/starter-hugo-academic" data-icon="octicon-star" data-size="large" data-show-count="true" aria-label="Star">Star the Academic template</a></div>
      text: |-

        Step into my world, the bringer of innovation,\
        where creativity and imagination collide.\
        My projects are like uncharted constellations,\
        waiting to be discovered in the vast realm of ideas.

        <!--Custom spacing-->
        <div class="mb-3"></div>
        <!--GitHub Button JS-->
        <script async defer src="https://buttons.github.io/buttons.js"></script>
    design:
      background:
        gradient_end: '#1976d2'
        gradient_start: '#004ba0'
        text_color_light: true
        image:
          filename: home-background.jpg

  - block: about.biography
    id: about
    content:
      title: Biography
      # Choose a user profile to display (a folder name within `content/authors/`)
      username: admin

  - block: features
    content:
      title: My OS Arsenal 🖥️
      items:
        - name: Arch Linux
          icon: archlinux
          icon_pack: custom
        - name: RHEL
          icon: rhel
          icon_pack: custom
        - name: OpenSUSE
          icon: opensuse
          icon_pack: custom
        - name: Debian
          icon: debian
          icon_pack: custom

  - block: features
    content:
      title: My Creative Cockpit 🛠️
      items:
        - name: VSCode
          icon: vscode
          icon_pack: custom
        - name: Sublime Text
          icon: sublime
          icon_pack: custom
        - name: Trae
          icon: trae
          icon_pack: custom
        - name: Windsurf IDE
          icon: windsurf
          icon_pack: custom

  - block: features
    content:
      title: Keeping it in sync 🔧
      items:
        - name: Git
          description:
          icon: git
          icon_pack: custom
        - name: ClearCase
          icon: clearcase
          icon_pack: custom
        - name: GitHub
          icon: github
          icon_pack: custom
        - name: BitBucket
          icon: bitbucket
          icon_pack: custom
        - name: Jira
          icon: jira
          icon_pack: custom
        - name: Confluence
          icon: confluence
          icon_pack: custom

  - block: features
    content:
      title: Virtualization Vibes 🌐
      items:
        - name: VMware Workstation
          icon: vmware-workstation
          icon_pack: custom
        - name: VirtualBox
          icon: virtualbox
          icon_pack: custom
        - name: Vagrant
          icon: vagrant
          icon_pack: custom

  - block: features
    content:
      title: Code I Speak 💻
      items:
        - name: Bash
          # description: Expert
          icon: bash
          icon_pack: custom
        - name: Python
          # description: Advanced
          icon: python
          icon_pack: custom
        - name: Golang
          # description: Intermediate
          icon: go
          icon_pack: custom
        - name: JavaScript
          # description: Intermediate
          icon: javascript
          icon_pack: custom
        - name: Markdown
          # description: Expert
          icon: markdown
          icon_pack: custom

  - block: features
    content:
      title: Frontend Flair & Frameworks 🖼️
      items:
        - name: Vue.js
          # description: Intermediate
          icon: vuejs
          icon_pack: custom
        - name: Bootstrap
          # description: Beginner
          icon: bootstrap
          icon_pack: custom
        - name: HTML
          icon: html
          icon_pack: custom
        - name: CSS
          icon: css
          icon_pack: custom

  - block: features
    content:
      title: Backend Brilliance ⚙️
      items:
        - name: Django
          icon: django
          icon_pack: custom
        - name: Django Rest Framework
          icon: django-rest
          icon_pack: custom
        - name: Gin
          icon: gin
          icon_pack: custom

  - block: features
    content:
      title: CI/CD & Container Craze 🔄
      items:
        - name: Docker
          # description: Advanced
          icon: docker
          icon_pack: custom
        - name: Podman
          icon: podman
          icon_pack: custom
        - name: Jenkins
          # description: Intermediate
          icon: jenkins
          icon_pack: custom
        - name: GitHub Actions
          # description: Advanced
          icon: gha
          icon_pack: custom
        - name: Kubernetes
          icon: kubernetes
          icon_pack: custom

  - block: features
    content:
      title: AI Arsenal 🤖
      items:
        - name: Claude
          icon: claude
          icon_pack: custom
        - name: Qwen
          icon: qwen
          icon_pack: custom
        - name: DeepSeek
          icon: deepseek
          icon_pack: custom
        - name: Grok
          icon: grok
          icon_pack: custom
        - name: Ollama
          icon: ollama
          icon_pack: custom
        - name: ChatGPT
          icon: chatgpt
          icon_pack: custom

  - block: features
    content:
      title: Soft Skills 🧠
      items:
        - name: AI Prompt Engineering
          description: Proficient in developing optimized prompts
        - name: Agile/Scrum Methodology
          description: Proficient in Agile project management frameworks and Scrum practices, including ceremonies and sprint management
        - name: Continuous Learning
          description: Committed to ongoing professional development and skill acquisition
        - name: Strategic Time Management
          description: Demonstrated ability to prioritize tasks and meet deadlines effectively
        - name: Professional Integrity
          description: Maintains high standards of self-discipline and accountability
        - name: Change Management
          description: Proven adaptability in dynamic work environments
        - name: Professional Excellence
          description: Dedicated to delivering quality results and maintaining workplace standards
        - name: Technical Problem-Solving
          description: Skilled in independent research and troubleshooting through strategic information gathering
        - name: Team Collaboration
          description: Strong ability to work collaboratively with team members and stakeholders

  - block: experience
    content:
      title: Experience
      # Date format for experience
      #   Refer to https://wowchemy.com/docs/customization/#date-format
      date_format: Jun 1, 2006
      # Experiences.
      #   Add/remove as many `experience` items below as you like.
      #   Required fields are `title`, `company`, and `date_start`.
      #   Leave `date_end` empty if it's your current employer.
      #   Begin multi-line descriptions with YAML's `|2-` multi-line prefix.
      items:
        - title: DevOps Engineer
          company: Strypes
          company_url: https://ict-strypes.eu/
          company_logo: strypes
          location: Varna
          date_start: '2022-06-01'
          date_end: ''
          description: |2-
              Responsibilities:

              * Automated manual processes using Python, Bash, and Go, reducing operational overhead and improving team efficiency
              * Designed and implemented development, testing, and deployment automation tools
              * Implemented CI/CD pipelines that accelerated deployment cycles
              * Migrated Jenkins pipelines to GitHub Actions workflows, modernizing CI/CD infrastructure
              * Built automated data pipeline for Splunk integration and created comprehensive monitoring dashboards
        - title: Software Development Trainee
          company: MentorMate
          company_url: https://mentormate.com
          company_logo: mentormate
          location: Varna
          date_start: '2022-02-02'
          date_end: '2022-03-15'
          description: |2-
              Responsibilities:

              * Developed frontend applications using TypeScript, Vue.js, HTML, CSS, SASS, and Bootstrap
              * Rapidly acquired new technical skills and adapted to evolving project requirements
              * Managed project timelines and delivered tasks according to established deadlines
        - title: Officer of the Watch (OOW)
          company: Stamco Manning Varna Co. Ltd.
          company_url: https://www.stamco.bg
          company_logo: stamco
          location: Varna
          date_start: '2015-06-01'
          date_end: '2022-01-01'
          description: |2-
              Responsibilities:

              * Maintained vessel and crew safety protocols in compliance with maritime regulations
              * Supported ship operations and organizational procedures during voyages
              * Supervised navigational watches and cargo operations as watch officer
              * Led and coordinated teams of crew members during operational duties
              * Demonstrated reliability and strong work ethic in demanding maritime environment
              * Managed critical time-sensitive operations and emergency response procedures
    design:
      columns: '2'
  - block: accomplishments
    content:
      # Note: `&shy;` is used to add a 'soft' hyphen in a long heading.
      title: Certificates
      subtitle:
      # Date format: https://wowchemy.com/docs/customization/#date-format
      date_format: Jan, 2006
      # Accomplishments.
      #   Add/remove as many `item` blocks below as you like.
      #   `title`, `organization`, and `date_start` are the required parameters.
      #   Leave other parameters empty if not required.
      #   Begin multi-line descriptions with YAML's `|2-` multi-line prefix.
      items:
        - certificate_url: https://softuni.bg/certificates/details/147847/a8898499
          date_end: '2022-11-21'
          date_start: '2022-09-20'
          description: ''
          organization: SoftUni
          organization_url: https://softuni.bg
          title: DevOps - Containerization, CI/CD & Monitoring
          url: ''
        - certificate_url: https://softuni.bg/certificates/details/131156/db558654
          date_end: '2022-04-19'
          date_start: '2022-02-22'
          description: ''
          organization: SoftUni
          organization_url: https://softuni.bg
          title: Python OOP
          url: ''
        - certificate_url: https://softuni.bg/certificates/details/126237/6f56edca
          date_end: '2022-04-15'
          date_start: '2022-01-11'
          description: ''
          organization: SoftUni
          organization_url: https://softuni.bg
          title: Python Advanced
          url: ''
        - certificate_url: https://softuni.bg/certificates/details/122964/cc388973
          date_end: '2022-01-31'
          date_start: '2021-11-24'
          description: ''
          organization: SoftUni
          organization_url: https://softuni.bg
          title: Linux System Administration
          url: ''
        - certificate_url: https://softuni.bg/certificates/details/118847/9b150c57
          date_end: '2021-11-22'
          date_start: '2021-09-29'
          description: ''
          organization: SoftUni
          organization_url: https://softuni.bg
          title: Windows System Administration
          url: ''
        - certificate_url: https://www.udemy.com/certificate/UC-012038b1-03ad-4fc8-a9dc-17dc020930fa/
          date_end: '2022-12-02'
          date_start: '2022-12-01'
          description: ''
          organization: Udemy
          organization_url: https://www.udemy.com
          title: GitHub Actions - The Complete Guide
          url: ''
        - certificate_url: https://softuni.bg/certificates/details/207384/ead50adc
          date_end: '2024-02-24'
          date_start: '2024-01-08'
          description: ''
          organization: SoftUni
          organization_url: https://softuni.bg
          title: Django Basics
          url: ''
    design:
      columns: '2'
  - block: collection
    id: posts
    content:
      title: Recent Posts
      subtitle: ''
      text: ''
      # Choose how many pages you would like to display (0 = all pages)
      count: 5
      # Filter on criteria
      filters:
        folders:
          - post
        author: ""
        category: ""
        tag: ""
        exclude_featured: false
        exclude_future: false
        exclude_past: false
        publication_type: ""
      # Choose how many pages you would like to offset by
      offset: 0
      # Page order: descending (desc) or ascending (asc) date.
      order: desc
    design:
      # Choose a layout view
      view: compact
      columns: '2'
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
        # - name: All
        #   tag: '*'
        - name: Python
          tag: Python
        - name: Web
          tag: Web
        - name: Scripts
          tag: Shell
          tag: Bash
        - name: Go
          tag: Go
        - name: Other
          tag: Other
    design:
      # Choose how many columns the section has. Valid values: '1' or '2'.
      columns: '2'
      view: showcase
      # For Showcase view, flip alternate rows?
      flip_alt_rows: false
  # - block: markdown
  #   content:
  #     title: Gallery
  #     subtitle: ''
  #     text: |-
  #       {{< gallery album="demo" >}}
  #   design:
  #     columns: '1'
  # - block: collection
  #   id: featured
  #   content:
  #     title: Featured Publications
  #     filters:
  #       folders:
  #         - publication
  #       featured_only: true
  #   design:
  #     columns: '2'
  #     view: card
  # - block: collection
  #   content:
  #     title: Recent Publications
  #     text: |-
  #       {{% callout note %}}
  #       Quickly discover relevant content by [filtering publications](./publication/).
  #       {{% /callout %}}
  #     filters:
  #       folders:
  #         - publication
  #       exclude_featured: true
  #   design:
  #     columns: '2'
  #     view: citation
  # - block: collection
  #   id: talks
  #   content:
  #     title: Recent & Upcoming Talks
  #     filters:
  #       folders:
  #         - event
  #   design:
  #     columns: '2'
  #     view: compact
  - block: tag_cloud
    content:
      title: Popular Topics
    design:
      columns: '2'
  - block: contact
    id: contact
    content:
      title: Contact
      subtitle:
      text: |-
        Please do not hesitate to contact me.
      # Contact (add or remove contact options as necessary)
      email: ivanov.iv.plamen@gmail.com
      phone: +359 892 758 777
      appointment_url: 'https://calendly.com/ivanov-iv-plamen'
      address:
        # street: 450 Serra Mall
        city: Varna
        region: Bulgaria
        # postcode: '94305'
        country: Bulgaria
        country_code: BG
      coordinates:
        latitude: '43.21667'
        longitude: '27.91667'
      # directions: Enter Building 1 and take the stairs to Office 200 on Floor 2
      # office_hours:
      #   - 'Monday 10:00 to 13:00'
      #   - 'Wednesday 09:00 to 10:00'
      contact_links:
        - icon: linkedin
          icon_pack: fab
          name: LinkedIn
          link: https://www.linkedin.com/in/plamen-i-ivanov/
        - icon: github
          icon_pack: fab
          link: https://github.com/k1lgor
          name: GitHub
        # - icon: twitter
        #   icon_pack: fab
        #   name: DM Me
        #   link: 'https://twitter.com/Twitter'
        # - icon: skype
        #   icon_pack: fab
        #   name: Skype Me
        #   link: 'skype:echo123?call'
        # - icon: video
        #   icon_pack: fas
        #   name: Zoom Me
        #   link: 'https://zoom.com'
      # Automatically link email and phone or display as text?
      autolink: true
      # Email form provider
      # form:
      #   provider: netlify
      #   formspree:
      #     id:
      #   netlify:
      #     # Enable CAPTCHA challenge to reduce spam?
      #     captcha: false
    design:
      columns: '2'
---
