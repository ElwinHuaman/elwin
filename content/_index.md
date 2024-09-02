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
      username: admin
      text: ""
      # Show a call-to-action button under your biography? (optional)
      button:
        text: Download CV
        url: uploads/Resume-ElwinHuaman.pdf
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
  - block: collection
    id: papers
    content:
      title: Featured Publications
      filters:
        folders:
          - publication
        featured_only: true
    design:
      view: article-grid
      columns: 3
  - block: collection
    id: projects
    content:
      title: Featured Projects
      filters:
        folders:
          - project
        featured_only: true
    design:
      view: article-grid
      columns: 3
  - block: collection
    id: talks
    content:
      title: Recent & Upcoming Talks
      filters:
        folders:
          - event
        featured_only: true
    design:
      view: article-grid
      columns: 2      
  - block: markdown
    content:
      title: '📚 Elwin Huaman Knowledge Graph'
      subtitle: 'powereded by [Wikidata](https://www.wikidata.org/entity/Q100324298)'
      text: '<iframe style="width: 80vw; height: 50vh; border: none;" src="https://query.wikidata.org/embed.html#%23%20tool%3A%20scholia%0APREFIX%20target%3A%20%3Chttp%3A%2F%2Fwww.wikidata.org%2Fentity%2FQ100324298%3E%0A%0A%23defaultView%3AGraph%0ASELECT%20%3Fnode%20%3FnodeLabel%20%3FnodeImage%20%3FchildNode%20%3FchildNodeLabel%20%3FchildNodeImage%20%3Frgb%20%0AWITH%20%7B%0A%20%20SELECT%20DISTINCT%20%3Fproperty%20WHERE%20%7B%0A%20%20%20%20%20%20%3Fproperty%20a%20wikibase%3AProperty%3B%0A%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20wdt%3AP31%20wd%3AQ18610173%20%3B%0A%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20wdt%3AP31%20wd%3AQ26940804%20.%20%0A%20%20%20%20%7D%0A%7D%20AS%20%25properties%0AWITH%20%7B%0A%20%20SELECT%20DISTINCT%20%3Fnode%20%3FchildNode%20WHERE%20%7B%0A%20%20%20%20%20%20BIND(target%3A%20AS%20%3Fnode)%0A%20%20%20%20%20%20%3Fnode%20%3Fp%20%3Fi.%0A%20%20%20%20%20%20%3FchildNode%20%3Fx%20%3Fp.%0A%20%20%20%20%20%20%3FchildNode%20rdf%3Atype%20wikibase%3AProperty.%0A%20%20%20%20%20%20FILTER(STRSTARTS(STR(%3Fi)%2C%20%22http%3A%2F%2Fwww.wikidata.org%2Fentity%2FQ%22))%0A%20%20%20%20%20%20FILTER(STRSTARTS(STR(%3FchildNode)%2C%20%22http%3A%2F%2Fwww.wikidata.org%2Fentity%2FP%22))%0A%20%20%20%20%7D%0A%20%20LIMIT%205000%0A%7D%20AS%20%25nodes%0AWITH%20%7B%0A%20%20SELECT%20DISTINCT%20%3FchildNode%20%3Fnode%20%3Frgb%20WHERE%20%7B%0A%20%20%20%20%20%20BIND(%22EFFBD8%22%20AS%20%3Frgb)%0A%20%20%20%20%20%20target%3A%20%3Fp%20%3FchildNode.%0A%20%20%20%20%20%20%3Fnode%20%3Fx%20%3Fp.%0A%20%20%20%20%20%20%3Fnode%20rdf%3Atype%20wikibase%3AProperty.%0A%20%20%20%20%20%20FILTER(STRSTARTS(STR(%3FchildNode)%2C%20%22http%3A%2F%2Fwww.wikidata.org%2Fentity%2FQ%22))%0A%20%20%20%20%7D%0A%20%20LIMIT%205000%0A%7D%20AS%20%25childNodes%0AWHERE%20%7B%0A%20%20%7B%0A%20%20%20%20INCLUDE%20%25nodes%0A%20%20%7D%0A%20%20UNION%0A%20%20%7B%0A%20%20%20%20INCLUDE%20%25childNodes%0A%20%20%7D%0A%0A%20%20OPTIONAL%20%7B%20%0A%20%20%20%20INCLUDE%20%25properties%0A%20%20%20%20%3Fproperty%20wikibase%3AdirectClaim%20%3Fnodeclaim.%0A%20%20%20%20%3Fnode%20%3Fnodeclaim%20%3FnodeImage.%20%0A%20%20%7D%0A%0A%20%20OPTIONAL%20%7B%20%0A%20%20%20%20INCLUDE%20%25properties%0A%20%20%20%20%3Fproperty%20wikibase%3AdirectClaim%20%3FchildNodeclaim.%0A%20%20%20%20%3FchildNode%20%3FchildNodeclaim%20%3FchildNodeImage.%20%0A%20%20%7D%0A%20%20%0A%20%20SERVICE%20wikibase%3Alabel%20%7B%20bd%3AserviceParam%20wikibase%3Alanguage%20%22%5BAUTO_LANGUAGE%5D%2Cen%22.%20%7D%20%20%20%20%20%20%20%20%0A%7D" referrerpolicy="origin" sandbox="allow-scripts allow-same-origin allow-popups"></iframe>'
    design:
      columns: '1'
  # - block: collection
  #   content:
  #     title: Recent Publications
  #     text: ""
  #     filters:
  #       folders:
  #         - publication
  #       exclude_featured: false
  #   design:
  #     view: citation
  - block: collection
    id: news
    content:
      title: Recent News
      subtitle: ''
      text: ''
      # Page type to display. E.g. post, talk, publication...
      page_type: post
      # Choose how many pages you would like to display (0 = all pages)
      count: 3
      # Filter on criteria
      filters:
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
      view: date-title-summary
      # Reduce spacing
      spacing:
        padding: [0, 0, 0, 0]
  - block: cta-card
    demo: true # Only display this section in the Hugo Blox Builder demo site
    content:
      title: 👉 Build your own academic website like this
      text: |-
        This site is generated by Hugo Blox Builder - the FREE, Hugo-based open source website builder trusted by 250,000+ academics like you.

        <a class="github-button" href="https://github.com/HugoBlox/hugo-blox-builder" data-color-scheme="no-preference: light; light: light; dark: dark;" data-icon="octicon-star" data-size="large" data-show-count="true" aria-label="Star HugoBlox/hugo-blox-builder on GitHub">Star</a>

        Easily build anything with blocks - no-code required!
        
        From landing pages, second brains, and courses to academic resumés, conferences, and tech blogs.
      button:
        text: Get Started
        url: https://hugoblox.com/templates/
    design:
      card:
        # Card background color (CSS class)
        css_class: "bg-primary-700"
        css_style: ""
---