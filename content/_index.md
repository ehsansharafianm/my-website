---
# Leave the homepage title empty to use the site title
title: ''
summary: ''
date: 2022-10-24
type: landing

sections:
  - block: resume-biography-3
    content:
      # Choose a user profile to display (a folder name within `content/authors/`)
      username: me
      text: ''
      # Show a call-to-action button under your biography? (optional)
      button:
        text: Download CV
        url: uploads/Ehsan-Sharafian-CV.pdf
      headings:
        about: ''
        education: ''
        interests: ''
    design:
      # Use the new Gradient Mesh which automatically adapts to the selected theme colors
      background:
        gradient_mesh:
          enable: true

      # Name heading sizing to accommodate long or short names
      name:
        size: md # Options: xs, sm, md, lg (default), xl

      # Avatar customization
      avatar:
        size: medium # Options: small (150px), medium (200px, default), large (320px), xl (400px), xxl (500px)
        shape: circle # Options: circle (default), square, rounded
  - block: markdown
    content:
      title: '📚 My Research'
      subtitle: ''
      text: |-
        I am a PhD candidate in Mechanical Engineering at the University of Maine's Biorobotics and Biomechanics Lab, supervised by Dr. Babak Hejrati. My research develops
        wearable IMU-based sensing systems for real-time gait analysis and fall prevention in older adults.

        My work spans distributed IMU networks, foot-clearance estimation, and adaptive haptic feedback, bridging laboratory research and real-world applications.

        Please reach out to collaborate. 
    design:
      columns: '1'

  - block: collection
    id: featured
    content:
      title: Featured Publications
      filters:
        folders:
          - publications
        featured_only: true
    design:
      view: article-grid
      columns: 3
  - block: collection
    id: papers
    content:
      title: Publications
      text: ''
      count: 0
      filters:
        folders:
          - publications
    design:
      view: citation

  - block: tech-stack
    id: skills
    content:
      title: Skills
      subtitle: Software and programming tools I work with
      categories:
        - name: Programming Languages
          items:
            - name: Python
              icon: devicon/python
            - name: C/C++
              icon: devicon/cplusplus
            - name: C#
              icon: devicon/csharp
            - name: Java
              icon: devicon/java
        - name: Relevant Software
          items:
            - name: MATLAB
              icon: devicon/matlab
            - name: Android Studio
              icon: devicon/androidstudio
            - name: SolidWorks
              icon: custom/solidworks
            - name: SPSS
              icon: devicon/spss
            - name: TwinCAT
              icon: custom/twincat
            - name: Adams
              icon: custom/adams  
            - name: Unity
              icon: devicon/unity
            - name: Blender
              icon: devicon/blender
    design:
      style: grid
      show_levels: false

  - block: resume-experience
    id: experience
    content:
      username: me
    design:
      date_format: 'Jan 2006'
      is_education_first: false
  - block: resume-experience
    id: academic-exp
    content:
      username: academic
    design:
      date_format: 'Jan 2006'
      is_education_first: false
  - block: collection
    id: projects
    content:
      title: Projects
      text: ''
      count: 0
      filters:
        folders:
          - projects
    design:
      view: article-grid
      columns: 2
  - block: collection
    id: talks
    content:
      title: Recent Talks
      filters:
        folders:
          - events
    design:
      view: article-grid
      columns: 2
---
