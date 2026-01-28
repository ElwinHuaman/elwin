---
# Leave the homepage title empty to use the site title
title: ""
date: 2022-10-24
type: landing

design:
  # Default section spacing
  spacing: "6rem"

sections:
  # - block: resume-biography-3
  #   content:
  #     # Choose a user profile to display (a folder name within `content/authors/`)
  #     username: elwin
  #     text: ""
  #     # Show a call-to-action button under your biography? (optional)
  #     button:
  #       text: Download Resume
  #       url: ../uploads/resume-ElwinHuaman.pdf
  #       # text: Download CV
  #       # url: uploads/resume.pdf
  #   design:
  #     css_class: dark
  #     background:
  #       color: black
  #       image:
  #         # Add your image background to `assets/media/`.
  #         # filename: stacked-peaks.svg
  #         filename: ElwinHuaman-Alpacas-2024.jpg
  #         filters:
  #           brightness: 0.7
  #         size: cover
  #         position: center
  #         parallax: false  
  - block: resume-biography-3
    content:
      # Choose a user profile to display (a folder name within `content/authors/`)
      username: elwin
      text: ''
      # Show a call-to-action button under your biography? (optional)
      button:
        text: Download Resume
        url: ../uploads/resume-ElwinHuaman.pdf
      headings:
        about: 'Contact Me 🪧'
        education: ''
        interests: ''
    design:
      # Use the new Gradient Mesh which automatically adapts to the selected theme colors
      background:
        gradient_mesh:
          enable: true

      # Name heading sizing to accommodate long or short names
      name:
        size: sm # Options: xs, sm, md, lg (default), xl

      # Avatar customization
      avatar:
        size: medium # Options: small (150px), medium (200px, default), large (320px), xl (400px), xxl (500px)
        shape: circle # Options: circle (default), square, rounded
---