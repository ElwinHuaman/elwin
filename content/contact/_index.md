---
# Leave the homepage title empty to use the site title
title: ""
date: 2022-10-24
type: landing

design:
  # Default section spacing
  spacing: "6rem"

sections:
  - block: resume-biography-3
    content:
      # Choose a user profile to display (a folder name within `content/authors/`)
      username: elwin
      text: ""
      # Show a call-to-action button under your biography? (optional)
      button:
        text: Download CV
        url: cv
        # text: Download CV
        # url: uploads/resume.pdf
    design:
      css_class: dark
      background:
        color: black
        image:
          # Add your image background to `assets/media/`.
          # filename: stacked-peaks.svg
          filename: ElwinHuaman-Alpacas-2024.jpg
          filters:
            brightness: 0.7
          size: cover
          position: center
          parallax: false  
---