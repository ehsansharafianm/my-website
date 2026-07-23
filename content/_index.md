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
        My research focuses on intelligent wearable systems for human movement analysis and digital health. I develop technologies that integrate wearable IMU sensing, haptic feedback, machine learning, biomechanical modeling, and real-time mobile applications to support gait analysis, activity recognition, fall prevention, and home-based rehabilitation.
        
        I am interested in bringing movement assessment beyond traditional laboratory and clinical settings by creating practical systems that provide real-time feedback and support mobility, rehabilitation, and independent living. My work combines hardware, software, and biomechanics, including Arduino-based prototypes, PCB modules, native Android applications, and data analysis pipelines in Python and MATLAB.
        
        My background also includes robotics, including surgical robotics, robot arms, parallel manipulators, kinematic and dynamic modeling, trajectory planning, control systems, and graphical user interfaces. This foundation continues to shape my approach to developing intelligent systems for healthcare and human movement applications.

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
                <span class="contact-txt"><span class="contact-lbl">University email · click to copy</span>ehsan.sharafian@maine.edu</span>
              </a>
              <a class="contact-row" href="mailto:ehsan.sharafian.m@gmail.com">
                <span class="contact-ic" aria-hidden="true">
                  <svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><rect x="2" y="4" width="20" height="16" rx="2"/><path d="m22 7-10 6L2 7"/></svg>
                </span>
                <span class="contact-txt"><span class="contact-lbl">Personal email · click to copy</span>ehsan.sharafian.m@gmail.com</span>
              </a>
            </div>
            <a class="contact-send" href="mailto:ehsan.sharafian@maine.edu">
              <svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" aria-hidden="true"><line x1="22" y1="2" x2="11" y2="13"/><polygon points="22 2 15 22 11 13 2 9 22 2"/></svg>
              Send an email
            </a>
          </div>
          <div class="contact-find">
            <p class="contact-find-lbl">FIND ME ON</p>
            <div class="contact-socials">
              <a href="https://github.com/ehsansharafianm" target="_blank" rel="noopener" aria-label="GitHub" title="GitHub"><svg viewBox="0 0 24 24" fill="currentColor" aria-hidden="true"><path d="M12 .297c-6.63 0-12 5.373-12 12 0 5.303 3.438 9.8 8.205 11.385.6.113.82-.258.82-.577 0-.285-.01-1.04-.015-2.04-3.338.724-4.042-1.61-4.042-1.61C4.422 18.07 3.633 17.7 3.633 17.7c-1.087-.744.084-.729.084-.729 1.205.084 1.838 1.236 1.838 1.236 1.07 1.835 2.809 1.305 3.495.998.108-.776.417-1.305.76-1.605-2.665-.3-5.466-1.332-5.466-5.93 0-1.31.465-2.38 1.235-3.22-.135-.303-.54-1.523.105-3.176 0 0 1.005-.322 3.3 1.23.96-.267 1.98-.399 3-.405 1.02.006 2.04.138 3 .405 2.28-1.552 3.285-1.23 3.285-1.23.645 1.653.24 2.873.12 3.176.765.84 1.23 1.91 1.23 3.22 0 4.61-2.805 5.625-5.475 5.92.42.36.81 1.096.81 2.22 0 1.606-.015 2.896-.015 3.286 0 .315.21.69.825.57C20.565 22.092 24 17.592 24 12.297c0-6.627-5.373-12-12-12"/></svg></a>
              <a href="https://www.linkedin.com/in/ehsan-sharafian-m" target="_blank" rel="noopener" aria-label="LinkedIn" title="LinkedIn"><svg viewBox="0 0 24 24" fill="currentColor" aria-hidden="true"><path d="M20.447 20.452h-3.554v-5.569c0-1.328-.027-3.037-1.852-3.037-1.853 0-2.136 1.445-2.136 2.939v5.667H9.351V9h3.414v1.561h.046c.477-.9 1.637-1.85 3.37-1.85 3.601 0 4.267 2.37 4.267 5.455v6.286zM5.337 7.433a2.062 2.062 0 0 1-2.063-2.065 2.064 2.064 0 1 1 2.063 2.065zm1.782 13.019H3.555V9h3.564v11.452zM22.225 0H1.771C.792 0 0 .774 0 1.729v20.542C0 23.227.792 24 1.771 24h20.451C23.2 24 24 23.227 24 22.271V1.729C24 .774 23.2 0 22.225 0z"/></svg></a>
              <a href="https://scholar.google.com/citations?user=IF_W5kkAAAAJ&hl=en" target="_blank" rel="noopener" aria-label="Google Scholar" title="Google Scholar"><svg viewBox="0 0 24 24" fill="currentColor" aria-hidden="true"><path d="M5.242 13.769L0 9.5 12 0l12 9.5-5.242 4.269C17.548 11.249 14.978 9.5 12 9.5c-2.977 0-5.548 1.748-6.758 4.269zM12 10a7 7 0 1 0 0 14 7 7 0 0 0 0-14z"/></svg></a>
              <a href="https://www.researchgate.net/profile/Ehsan-Sharafian-Moghaddam" target="_blank" rel="noopener" aria-label="ResearchGate" title="ResearchGate"><svg viewBox="0 0 24 24" fill="currentColor" aria-hidden="true"><path d="M19.586 0c-.818 0-1.508.19-2.073.565-.563.377-.997.936-1.303 1.678-.302.741-.454 1.65-.454 2.727v.006c0 1.074.152 1.98.454 2.72.306.74.74 1.302 1.303 1.68.565.376 1.255.564 2.073.564.8 0 1.482-.188 2.05-.565.573-.377 1.01-.938 1.314-1.68.303-.74.454-1.646.454-2.72v-.006c0-1.076-.151-1.986-.454-2.727-.303-.742-.741-1.301-1.314-1.678C21.068.19 20.386 0 19.586 0zm.007 1.256c.415 0 .764.104 1.049.31.285.208.5.51.647.905.145.396.219.87.219 1.418v.007c0 .548-.074 1.02-.22 1.416-.146.395-.361.696-.646.902-.285.206-.634.31-1.049.31-.415 0-.766-.104-1.05-.31-.286-.206-.502-.507-.649-.902-.146-.396-.219-.868-.219-1.416v-.007c0-.548.073-1.022.22-1.418.146-.394.362-.697.648-.904.284-.207.635-.31 1.05-.31zM0 4.373v15.254A4.372 4.372 0 0 0 4.373 24h15.254A4.372 4.372 0 0 0 24 19.627v-6.873a4.996 4.996 0 0 1-1.794 1.383v5.49a2.578 2.578 0 0 1-2.579 2.579H4.373a2.578 2.578 0 0 1-2.579-2.579V4.373a2.578 2.578 0 0 1 2.579-2.579h9.208c.056-.624.209-1.201.442-1.72A4.4 4.4 0 0 0 4.373 0 4.372 4.372 0 0 0 0 4.373z"/></svg></a>
              <a href="https://orcid.org/0009-0001-8165-7375" target="_blank" rel="noopener" aria-label="ORCID" title="ORCID"><svg viewBox="0 0 24 24" fill="currentColor" aria-hidden="true"><path d="M12 0C5.372 0 0 5.372 0 12s5.372 12 12 12 12-5.372 12-12S18.628 0 12 0zM7.369 4.378c.525 0 .947.431.947.947 0 .525-.422.947-.947.947a.95.95 0 0 1-.946-.947c0-.516.421-.947.946-.947zm-.722 3.038h1.444v10.041H6.647V7.416zm3.562 0h3.9c3.712 0 5.344 2.653 5.344 5.025 0 2.578-2.016 5.025-5.325 5.025h-3.919V7.416zm1.444 1.303v7.444h2.297c3.272 0 4.022-2.484 4.022-3.722 0-2.016-1.284-3.722-4.097-3.722h-2.222z"/></svg></a>
            </div>
          </div>
        </div>
    design:
      columns: '1'
---
