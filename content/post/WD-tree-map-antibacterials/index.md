---
# Documentation: https://wowchemy.com/docs/managing-content/

title: "WD Tree Map Antibacterials"
subtitle: ""
summary: ""
authors: []
tags: []
categories: []
date: 2021-02-16T16:38:58+01:00
lastmod: 2021-02-16T16:38:58+01:00
featured: false
draft: false

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder.
# Focal points: Smart, Center, TopLeft, Top, TopRight, Left, Right, BottomLeft, Bottom, BottomRight.
image:
  caption: ""
  focal_point: ""
  preview_only: false

# Projects (optional).
#   Associate this post with one or more of your projects.
#   Simply enter your project's folder or file name without extension.
#   E.g. `projects = ["internal-project"]` references `content/project/deep-learning/index.md`.
#   Otherwise, set `projects = []`.
projects: []
---


SPARQL queries are not necessarily rendered as tables ... have a look at this 🌳 🗺️ 

<!--more-->

The folowing Wikidata SPAQRL query will retrieve all compounds found having the MESH property "antibacterial" associated. The results are counted and grouped at the taxa and parent taxa level of the containing organism. The results are outputted as a treemamp.



<iframe style="width: 80vw; height: 50vh; border: none;" src="https://query.wikidata.org/embed.html#%23defaultView%3ATreeMap%0ASELECT%20DISTINCT%20%3Fparent_taxon%20%3Fparent_taxon_name%20%3Ftaxon%20%3Ftaxon_name%20%20(COUNT(%3Fcompound)%20AS%20%3Fcount)%20WHERE%20%7B%0A%20%20%3Fcompound%20wdt%3AP2868%20%3Fmesh.%0A%20%20%3Fmesh%20wdt%3AP486%20%22D000900%22.%0A%20%20%3Fcompound%20wdt%3AP235%20%3Finchikey.%0A%20%20%7B%0A%20%20%20%20%3Fcompound%20p%3AP703%20%3Fstatement.%0A%20%20%20%20%3Fstatement%20ps%3AP703%20%3Ftaxon.%0A%20%20%20%20%3Ftaxon%20wdt%3AP171%20%3Fparent_taxon.%0A%20%20%20%20OPTIONAL%20%7B%20%3Ftaxon%20wdt%3AP171%20%3Fparent_taxon.%20%7D%0A%20%20%20%20OPTIONAL%20%7B%20%3Fparent_taxon%20wdt%3AP225%20%3Fparent_taxon_name.%20%7D%0A%20%20%20%20OPTIONAL%20%7B%20%3Ftaxon%20wdt%3AP225%20%3Ftaxon_name.%20%7D%0A%20%20%20%20%7B%0A%20%20%20%20%20%20%3Fstatement%20prov%3AwasDerivedFrom%20%3Fref.%0A%20%20%20%20%20%20%3Fref%20pr%3AP248%20%3Freference.%0A%20%20%20%20%20%20%3Freference%20wdt%3AP356%20%3Freference_doi%3B%0A%20%20%20%20%20%20%20%20wdt%3AP1476%20%3Freference_title.%0A%20%20%20%20%7D%0A%20%20%7D%0A%20%20SERVICE%20wikibase%3Alabel%20%7B%20bd%3AserviceParam%20wikibase%3Alanguage%20%22%5BAUTO_LANGUAGE%5D%2Cen%22.%20%7D%0A%7D%0AGROUP%20BY%20%20%3Fparent_taxon%20%3Fparent_taxon_name%20%3Ftaxon%20%3Ftaxon_name%0AORDER%20BY%20DESC%20(%3Fcount)%0ALIMIT%2070" referrerpolicy="origin" sandbox="allow-scripts allow-same-origin allow-popups"></iframe>
