---
title: 'Experience'
date: 2023-10-24
type: landing

design:
  spacing: '5rem'

# Note: `username` refers to the user's folder name in `content/authors/`

# Page sections
sections:
  - block: resume-experience
    content:
      username: me
    design:
      # Hugo date format
      date_format: 'Jan 2006'
      # Education or Experience section first?
      is_education_first: true

  - block: markdown
    content:
      title: 'Academic Experience'
      text: |-
        ### Laboratory Research Assistant
        **New Technology Research Center (NTRC), Amirkabir University of Technology** · Nov 2021 – Present

        - Assisted in conducting undergraduate research projects
        - Provided laboratory services for graduate students
        - Maintained laboratory equipment and coordinated repairs
        - Helped organize the 9th RSI International Conference on Robotics and Mechatronics (ICROM)
    design:
      columns: '1'
  - block: resume-skills
    content:
      title: Hobbies
      username: me
  - block: resume-awards
    id: awards
    content:
      title: Awards
      username: me
  - block: resume-languages
    content:
      title: Languages
      username: me
---
