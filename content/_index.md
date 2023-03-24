---
# Leave the homepage title empty to use the site title
title:
date: 2022-10-24
type: landing

sections:
  - block: about.avatar
    id: about
    content:
      # Choose a user profile to display (a folder name within `content/authors/`)
      username: admin
      # Override your bio text from `authors/admin/_index.md`?
      text:
  - block: features
    content:
      title: Skills
      items:
        - name: OCT imaging
          icon: r-project
          icon_pack: fab
        - name: OCT Angiography (OCTA) 
          icon: chart-line
          icon_pack: fas
        - name: Intrinsic Optical Signalling
          icon: camera-retro
          icon_pack: fas
        - name: Polymer Chemistry
          icon: camera-retro
          icon_pack: fas
        - name: Experimental Design
          icon: camera-retro
          icon_pack: fas
        - name: Scientific Communication
          icon: camera-retro
          icon_pack: fas
        - name: Teaching and Mentorship
          icon: camera-retro
          icon_pack: fas
        - name: Data analysis and Statistics
          icon: camera-retro
          icon_pack: fas
  - block: experience
    content:
      title: Experience
      # Date format for experience
      #   Refer to https://wowchemy.com/docs/customization/#date-format
      date_format: Jan 2006
      # Experiences.
      #   Add/remove as many `experience` items below as you like.
      #   Required fields are `title`, `company`, and `date_start`.
      #   Leave `date_end` empty if it's your current employer.
      #   Begin multi-line descriptions with YAML's `|2-` multi-line prefix.
      items:
        - title: Graduate Research Assistant
          company: University of Illinois at Chicago
          company_url: ''
          company_logo: org-gc
          location: Chicago
          date_start: '2018-09-01'
          date_end: ''
          description: |2-
              Concentrating on cutting-edge ophthalmic equipment and quantitative imaging techniques to propel
              retinal research, disease identification, and treatment assessment. Laboratory investigations 
              involve extensive field fundus imaging, functional Optical Coherence Tomography (OCT), quantitative
              OCT angiography (OCTA), high-resolution ophthalmoscopy, functional imaging of neurovascular
              interactions, image analysis employing machine learning, and artificial intelligence-based
              categorization.
       - title: Graduate Research Assistant
          company: University of Illinois at Chicago
          company_url: ''
          company_logo: org-gc
          location: Chicago
          date_start: '2018-09-01'
          date_end: ''
          description: |2-
              Concentrating on cutting-edge ophthalmic equipment and quantitative imaging techniques to propel
              retinal research, disease identification, and treatment assessment. Laboratory investigations 
              involve extensive field fundus imaging, functional Optical Coherence Tomography (OCT), quantitative
              OCT angiography (OCTA), high-resolution ophthalmoscopy, functional imaging of neurovascular
              interactions, image analysis employing machine learning, and artificial intelligence-based
              categorization.
        - title: Science Teacher
          company: Beijing Nantional Day School
          company_url: ''
          company_logo: org-x
          location: Beijing
          date_start: '2013-09-01'
          date_end: '2018-07-31'
          description:  
          Well-rounded and passionate educator
          Experienced in teaching chemistry, biology, physics, geography, and mathematics
          College-level teaching experience
          Emphasizes practical applications of scientific principles
          Encourages critical thinking and problem-solving
          Shares insights from personal research experience
          Inspires curiosity and exploration in students
          Fosters strong teacher-student relationships
          Creates engaging lesson plans and learning environments
    
    
    design:
      columns: '3'
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
        - name: All
          tag: '*'
    design:
      # Choose how many columns the section has. Valid values: '1' or '2'.
      columns: '1'
      view: showcase
      # For Showcase view, flip alternate rows?
      flip_alt_rows: false
  - block: markdown
    content:
      title: Gallery
      subtitle: ''
      text: |-
        {{< gallery album="demo" >}}
    design:
      columns: '1'
  - block: collection
    id: featured
    content:
      title: Featured Publications
      filters:
        folders:
          - publication
        featured_only: true
    design:
      columns: '2'
      view: card
  - block: collection
    content:
      title: Recent Publications
      text: |-
        {{% callout note %}}
        Quickly discover relevant content by [filtering publications](./publication/).
        {{% /callout %}}
      filters:
        folders:
          - publication
        exclude_featured: true
    design:
      columns: '2'
      view: citation
  - block: collection
    id: talks
    content:
      title: Recent & Upcoming Talks
      filters:
        folders:
          - event
    design:
      columns: '2'
      view: compact
  - block: tag_cloud
    content:
      title: Popular Topics
    design:
      columns: '2'

---
