---
# An instance of the About widget.
# Documentation: https://wowchemy.com/docs/page-builder/
widget: "blank"

# Activate this widget? true/false
active: true

# This file represents a page section.
headless: true

# Order that this section appears on the page.
weight: 25

title: Elwin Huaman Knowledge Graph
subtitle: 'powered by [Wikidata](https://www.wikidata.org/entity/Q100324298)'

# Choose the user profile to display
# This should be the username (folder name) of a profile in your `content/authors/` folder.
# See https://wowchemy.com/docs/get-started/#introduce-yourself
author: admin

design:
      # See Page Builder docs for all section customization options.
      # Choose how many columns the section has. Valid values: '1' or '2'.
      columns: '1'
---
<iframe style="width: 80vw; height: 50vh; border: none;" src="https://query.wikidata.org/embed.html#%23%20tool%3A%20scholia%0APREFIX%20target%3A%20%3Chttp%3A%2F%2Fwww.wikidata.org%2Fentity%2FQ100324298%3E%0A%0A%23defaultView%3AGraph%0ASELECT%20%3Fnode%20%3FnodeLabel%20%3FnodeImage%20%3FchildNode%20%3FchildNodeLabel%20%3FchildNodeImage%20%3Frgb%20%0AWITH%20%7B%0A%20%20SELECT%20DISTINCT%20%3Fproperty%20WHERE%20%7B%0A%20%20%20%20%20%20%3Fproperty%20a%20wikibase%3AProperty%3B%0A%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20wdt%3AP31%20wd%3AQ18610173%20%3B%0A%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20wdt%3AP31%20wd%3AQ26940804%20.%20%0A%20%20%20%20%7D%0A%7D%20AS%20%25properties%0AWITH%20%7B%0A%20%20SELECT%20DISTINCT%20%3Fnode%20%3FchildNode%20WHERE%20%7B%0A%20%20%20%20%20%20BIND(target%3A%20AS%20%3Fnode)%0A%20%20%20%20%20%20%3Fnode%20%3Fp%20%3Fi.%0A%20%20%20%20%20%20%3FchildNode%20%3Fx%20%3Fp.%0A%20%20%20%20%20%20%3FchildNode%20rdf%3Atype%20wikibase%3AProperty.%0A%20%20%20%20%20%20FILTER(STRSTARTS(STR(%3Fi)%2C%20%22http%3A%2F%2Fwww.wikidata.org%2Fentity%2FQ%22))%0A%20%20%20%20%20%20FILTER(STRSTARTS(STR(%3FchildNode)%2C%20%22http%3A%2F%2Fwww.wikidata.org%2Fentity%2FP%22))%0A%20%20%20%20%7D%0A%20%20LIMIT%205000%0A%7D%20AS%20%25nodes%0AWITH%20%7B%0A%20%20SELECT%20DISTINCT%20%3FchildNode%20%3Fnode%20%3Frgb%20WHERE%20%7B%0A%20%20%20%20%20%20BIND(%22EFFBD8%22%20AS%20%3Frgb)%0A%20%20%20%20%20%20target%3A%20%3Fp%20%3FchildNode.%0A%20%20%20%20%20%20%3Fnode%20%3Fx%20%3Fp.%0A%20%20%20%20%20%20%3Fnode%20rdf%3Atype%20wikibase%3AProperty.%0A%20%20%20%20%20%20FILTER(STRSTARTS(STR(%3FchildNode)%2C%20%22http%3A%2F%2Fwww.wikidata.org%2Fentity%2FQ%22))%0A%20%20%20%20%7D%0A%20%20LIMIT%205000%0A%7D%20AS%20%25childNodes%0AWHERE%20%7B%0A%20%20%7B%0A%20%20%20%20INCLUDE%20%25nodes%0A%20%20%7D%0A%20%20UNION%0A%20%20%7B%0A%20%20%20%20INCLUDE%20%25childNodes%0A%20%20%7D%0A%0A%20%20OPTIONAL%20%7B%20%0A%20%20%20%20INCLUDE%20%25properties%0A%20%20%20%20%3Fproperty%20wikibase%3AdirectClaim%20%3Fnodeclaim.%0A%20%20%20%20%3Fnode%20%3Fnodeclaim%20%3FnodeImage.%20%0A%20%20%7D%0A%0A%20%20OPTIONAL%20%7B%20%0A%20%20%20%20INCLUDE%20%25properties%0A%20%20%20%20%3Fproperty%20wikibase%3AdirectClaim%20%3FchildNodeclaim.%0A%20%20%20%20%3FchildNode%20%3FchildNodeclaim%20%3FchildNodeImage.%20%0A%20%20%7D%0A%20%20%0A%20%20SERVICE%20wikibase%3Alabel%20%7B%20bd%3AserviceParam%20wikibase%3Alanguage%20%22%5BAUTO_LANGUAGE%5D%2Cen%22.%20%7D%20%20%20%20%20%20%20%20%0A%7D" referrerpolicy="origin" sandbox="allow-scripts allow-same-origin allow-popups"></iframe>