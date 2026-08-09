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
        text: Resume
        url: uploads/Ehsan-Sharafian-Resume.pdf
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
        My research focuses on intelligent wearable systems for human movement analysis and digital health. I develop technologies that integrate wearable IMU sensing, haptic feedback, machine learning, biomechanical modeling, and real-time mobile applications to support gait analysis, activity recognition, fall prevention, and home-based rehabilitation.
        
        I am interested in bringing movement assessment beyond traditional laboratory and clinical settings by creating practical systems that provide real-time feedback and support mobility, rehabilitation, and independent living. My work combines hardware, software, and biomechanics, including Arduino-based prototypes, PCB modules, native Android applications, and data analysis pipelines in Python and MATLAB.
        
        My background also includes robotics, including surgical robotics, robot arms, parallel manipulators, kinematic and dynamic modeling, trajectory planning, control systems, and graphical user interfaces. This foundation continues to shape my approach to developing intelligent systems for healthcare and human movement applications.

    design:
      columns: '1'

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
  - block: collection
    id: hobbies
    content:
      title: Hobbies
      text: "Life outside the lab: camping, mountain trails, road trips, and working on my car."
      count: 0
      filters:
        folders:
          - hobbies
    design:
      view: article-grid
      columns: 2
  - block: markdown
    id: contact
    content:
      title: 'Get in Touch'
      subtitle: "I'm always open to research collaborations and conversations"
      text: |-
        <div class="contact-card">
          <div class="contact-connect">
            <h3>Connect</h3>
            <p>Whether you'd like to discuss research, explore a collaboration, or simply say hello, please feel free to reach out. I'll do my best to respond promptly.</p>
            <div class="contact-list">
              <a class="contact-row" href="tel:+12076316979">
                <span class="contact-ic" aria-hidden="true">
                  <svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M22 16.92v3a2 2 0 0 1-2.18 2 19.79 19.79 0 0 1-8.63-3.07 19.5 19.5 0 0 1-6-6 19.79 19.79 0 0 1-3.07-8.67A2 2 0 0 1 4.11 2h3a2 2 0 0 1 2 1.72c.13.94.36 1.86.68 2.75a2 2 0 0 1-.45 2.11L8.09 9.91a16 16 0 0 0 6 6l1.33-1.33a2 2 0 0 1 2.11-.45c.89.32 1.81.55 2.75.68A2 2 0 0 1 22 16.92z"/></svg>
                </span>
                <span class="contact-txt"><span class="contact-lbl">Phone</span>(207) 631-6979</span>
              </a>
              <a class="contact-row" href="mailto:ehsan.sharafian@maine.edu">
                <span class="contact-ic" aria-hidden="true">
                  <svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><rect x="2" y="4" width="20" height="16" rx="2"/><path d="m22 7-10 6L2 7"/></svg>
                </span>
                <span class="contact-txt"><span class="contact-lbl">University email</span>ehsan.sharafian@maine.edu</span>
              </a>
              <a class="contact-row" href="mailto:ehsan.sharafian.m@gmail.com">
                <span class="contact-ic" aria-hidden="true">
                  <svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><rect x="2" y="4" width="20" height="16" rx="2"/><path d="m22 7-10 6L2 7"/></svg>
                </span>
                <span class="contact-txt"><span class="contact-lbl">Personal email</span>ehsan.sharafian.m@gmail.com</span>
              </a>
            </div>
          </div>
          <div class="contact-find">
            <p class="contact-find-lbl">FIND ME ON</p>
            <div class="contact-socials">
              <a href="https://github.com/ehsansharafianm" target="_blank" rel="noopener" aria-label="GitHub" title="GitHub"><svg viewBox="0 0 24 24" fill="currentColor" aria-hidden="true"><path d="M12 .297c-6.63 0-12 5.373-12 12 0 5.303 3.438 9.8 8.205 11.385.6.113.82-.258.82-.577 0-.285-.01-1.04-.015-2.04-3.338.724-4.042-1.61-4.042-1.61C4.422 18.07 3.633 17.7 3.633 17.7c-1.087-.744.084-.729.084-.729 1.205.084 1.838 1.236 1.838 1.236 1.07 1.835 2.809 1.305 3.495.998.108-.776.417-1.305.76-1.605-2.665-.3-5.466-1.332-5.466-5.93 0-1.31.465-2.38 1.235-3.22-.135-.303-.54-1.523.105-3.176 0 0 1.005-.322 3.3 1.23.96-.267 1.98-.399 3-.405 1.02.006 2.04.138 3 .405 2.28-1.552 3.285-1.23 3.285-1.23.645 1.653.24 2.873.12 3.176.765.84 1.23 1.91 1.23 3.22 0 4.61-2.805 5.625-5.475 5.92.42.36.81 1.096.81 2.22 0 1.606-.015 2.896-.015 3.286 0 .315.21.69.825.57C20.565 22.092 24 17.592 24 12.297c0-6.627-5.373-12-12-12"/></svg></a>
              <a href="https://www.linkedin.com/in/ehsan-sharafian-m" target="_blank" rel="noopener" aria-label="LinkedIn" title="LinkedIn"><svg viewBox="0 0 24 24" fill="currentColor" aria-hidden="true"><path d="M20.447 20.452h-3.554v-5.569c0-1.328-.027-3.037-1.852-3.037-1.853 0-2.136 1.445-2.136 2.939v5.667H9.351V9h3.414v1.561h.046c.477-.9 1.637-1.85 3.37-1.85 3.601 0 4.267 2.37 4.267 5.455v6.286zM5.337 7.433a2.062 2.062 0 0 1-2.063-2.065 2.064 2.064 0 1 1 2.063 2.065zm1.782 13.019H3.555V9h3.564v11.452zM22.225 0H1.771C.792 0 0 .774 0 1.729v20.542C0 23.227.792 24 1.771 24h20.451C23.2 24 24 23.227 24 22.271V1.729C24 .774 23.2 0 22.225 0z"/></svg></a>
              <a href="https://scholar.google.com/citations?user=IF_W5kkAAAAJ&hl=en" target="_blank" rel="noopener" aria-label="Google Scholar" title="Google Scholar"><svg viewBox="0 0 24 24" fill="currentColor" aria-hidden="true"><path d="M5.242 13.769L0 9.5 12 0l12 9.5-5.242 4.269C17.548 11.249 14.978 9.5 12 9.5c-2.977 0-5.548 1.748-6.758 4.269zM12 10a7 7 0 1 0 0 14 7 7 0 0 0 0-14z"/></svg></a>
              <a href="https://www.researchgate.net/profile/Ehsan-Sharafian-Moghaddam" target="_blank" rel="noopener" aria-label="ResearchGate" title="ResearchGate"><svg viewBox="0 0 384 512" fill="currentColor" aria-hidden="true"><path d="M228.66 408.101c-20.194-21.973-47.218-57.268-69.698-97.166c37.134-8.685 64.633-43.55 64.633-78.384c0-51.345-39.88-75.176-92.163-75.176c-27.023 0-48.583 1.365-68.716 1.365c-18.369 0-36.722 0-48.154-.445V171.6l17.401 3.192c11.97 2.302 18.783 7.765 18.783 36.214v180.6c0 28.435-6.813 33.928-18.783 36.2l-17.4 3.252v13.259c12.367-.445 33.912-1.351 55.473-1.351c20.624 0 47.217.906 58.68 1.35v-13.258l-23.847-3.253c-12.366-1.796-18.813-7.764-18.813-36.2v-76.542c11.002.921 20.624.921 35.325.921c27.96 49.95 54.551 87.56 69.652 104.962c13.78 16.526 34.85 27.054 61.442 27.054c7.781 0 16.023-1.367 21.054-3.683v-11.894c-16.496 0-32.992-11.477-44.87-24.321zM119.064 295.344c-15.591 0-22.434-.414-33.008-1.41V178.918c10.574-.92 24.752-.92 37.136-.92c38.531 0 61.427 20.195 61.427 56.839c0 36.215-24.736 60.506-65.555 60.506M258.998 179.64c-.46-2.409-.875-5.217-1.243-8.456c-.383-3.268-.63-7.104-.782-11.63c-.154-4.496-.215-9.99-.215-16.282c0-6.323.061-11.74.215-16.25c.152-4.528.399-8.41.782-11.648c.368-3.223.782-6.046 1.243-8.455a51 51 0 0 1 1.78-6.982c3.943-11.923 10.405-20.885 19.443-26.901C289.244 67.02 300.308 64 313.443 64c6.752 0 12.875.782 18.307 2.377c5.371 1.581 10.189 3.76 14.44 6.553c4.189 2.762 7.81 6.015 10.802 9.698a53 53 0 0 1 7.474 11.878c.75 1.35.537 2.425-.66 3.176l-16.68 6.858c-1.413.753-2.41.37-3.193-1.12c-3.743-6.936-6.936-11.493-12.183-14.807c-5.31-3.3-10.22-4.865-18.308-4.865c-8.793 0-12.721 1.749-18.23 5.693c-5.463 3.867-9.468 8.732-11.832 16.143c-.474 1.335-.905 2.993-1.41 4.942c-.415 1.98-.753 4.404-.967 7.242c-.215 2.84-.415 6.353-.598 10.497c-.123 4.144-.184 9.177-.184 15.008c0 5.86.061 10.894.184 15.038c.184 4.128.383 7.641.598 10.48c.214 2.87.552 5.279.966 7.274c.507 1.919.937 3.575 1.411 4.927c2.364 7.38 5.74 11.415 10.712 14.654c4.911 3.284 10.557 5.648 19.35 5.648c7.811 0 14.962-2.225 19.626-5.618c4.62-3.39 8.456-7.87 10.175-13.994c.753-2.579 1.72-5.786 2.38-9.714c.598-3.929.598-8.087.598-13.825c0-.907-.508-1.367-1.352-1.367h-26.716c-1.504 0-2.24-.736-2.24-2.24v-15.314c0-1.52.736-2.257 2.24-2.257h49.028c1.535 0 2.257.737 2.257 2.257v13.09c0 6.935 0 13.365-.722 19.32c-.691 5.953-1.626 11.109-2.808 14.868c-3.744 11.77-9.682 20.15-18.782 26.394c-9.131 6.291-20.9 9.682-33.684 9.682c-13.135 0-24.199-3.022-33.221-9.022c-9.039-6.077-15.5-14.993-19.443-26.916a51 51 0 0 1-1.78-6.997z"/></svg></a>
              <a href="https://orcid.org/0009-0001-8165-7375" target="_blank" rel="noopener" aria-label="ORCID" title="ORCID"><svg viewBox="0 0 24 24" fill="currentColor" aria-hidden="true"><path d="M12 0C5.372 0 0 5.372 0 12s5.372 12 12 12 12-5.372 12-12S18.628 0 12 0zM7.369 4.378c.525 0 .947.431.947.947 0 .525-.422.947-.947.947a.95.95 0 0 1-.946-.947c0-.516.421-.947.946-.947zm-.722 3.038h1.444v10.041H6.647V7.416zm3.562 0h3.9c3.712 0 5.344 2.653 5.344 5.025 0 2.578-2.016 5.025-5.325 5.025h-3.919V7.416zm1.444 1.303v7.444h2.297c3.272 0 4.022-2.484 4.022-3.722 0-2.016-1.284-3.722-4.097-3.722h-2.222z"/></svg></a>
              <a href="https://www.youtube.com/@ehsansharafian" target="_blank" rel="noopener" aria-label="YouTube" title="YouTube"><svg viewBox="0 0 24 24" fill="currentColor" aria-hidden="true"><path d="M23.498 6.186a3.016 3.016 0 0 0-2.122-2.136C19.505 3.545 12 3.545 12 3.545s-7.505 0-9.377.505A3.017 3.017 0 0 0 .502 6.186C0 8.07 0 12 0 12s0 3.93.502 5.814a3.016 3.016 0 0 0 2.122 2.136c1.871.505 9.376.505 9.376.505s7.505 0 9.377-.505a3.015 3.015 0 0 0 2.122-2.136C24 15.93 24 12 24 12s0-3.93-.502-5.814zM9.545 15.568V8.432L15.818 12l-6.273 3.568z"/></svg></a>
            </div>
          </div>
        </div>
    design:
      columns: '1'
---
