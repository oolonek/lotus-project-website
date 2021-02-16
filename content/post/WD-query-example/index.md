---
# Documentation: https://wowchemy.com/docs/managing-content/

title: "Virola compounds - a SPARQL query example"
subtitle: ""
summary: ""
authors: []
tags: []
categories: []
date: 2021-02-16T15:49:43+01:00
lastmod: 2021-02-16T15:49:43+01:00
featured: true
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

An embedded wd query example

<!--more-->

The folowing Wikidata SPAQRL query will retrieve all compounds found in taxa whose parent taxon name is _"Virola"._


<div class="container">
        <div id="one-tab-content">
            <h5 class="title is-5" style="text-align:center;"> <i>Virola</i> genus compounds </h5>
        <div class="columns is-centered"
        <p style="text-align: center">
            <iframe width=120% height="600" src="https://query.wikidata.org/embed.html#SELECT%20DISTINCT%20%3Fcompound%20%3FcompoundLabel%20%3Finchikey%20%3Finchi%20%3Fsmiles_isomeric%20%3Fsmiles_canonical%20%3Fcas%20%3Fchebi%20%3Fchembl%20%3Fpubchem%20%3Ftaxon%20%3Ftaxon_name%20%3Ftaxon_id_gbif%20%3Ftaxon_id_ncbi%20%3Freference%20%3Freference_doi%20%3Freference_title%20WHERE%20%7B%0A%20%20%3Ftaxon%20wdt%3AP171%20%3Fparent_taxon.%0A%20%20%3Fparent_taxon%20wdt%3AP225%20%27Virola%27.%0A%20%20%3Fcompound%20wdt%3AP235%20%3Finchikey.%0A%20%20OPTIONAL%20%7B%20%3Fcompound%20wdt%3AP231%20%3Fcas.%20%7D%0A%20%20OPTIONAL%20%7B%20%3Fcompound%20wdt%3AP233%20%3Fsmiles_canonical.%20%7D%0A%20%20OPTIONAL%20%7B%20%3Fcompound%20wdt%3AP234%20%3Finchi.%20%7D%0A%20%20OPTIONAL%20%7B%20%3Fcompound%20wdt%3AP592%20%3Fchembl.%20%7D%0A%20%20OPTIONAL%20%7B%20%3Fcompound%20wdt%3AP662%20%3Fpubchem.%20%7D%0A%20%20OPTIONAL%20%7B%20%3Fcompound%20wdt%3AP683%20%3Fchebi.%20%7D%0A%20%20OPTIONAL%20%7B%20%3Fcompound%20wdt%3AP2017%20%3Fsmiles_isomeric.%20%7D%0A%20%20%7B%0A%20%20%20%20%3Fcompound%20p%3AP703%20%3Fstatement.%0A%20%20%20%20%3Fstatement%20ps%3AP703%20%3Ftaxon.%0A%20%20%20%20OPTIONAL%20%7B%20%3Ftaxon%20wdt%3AP225%20%3Ftaxon_name.%20%7D%0A%20%20%20%20OPTIONAL%20%7B%20%3Ftaxon%20wdt%3AP846%20%3Ftaxon_id_gbif.%20%7D%0A%20%20%20%20OPTIONAL%20%7B%20%3Ftaxon%20wdt%3AP685%20%3Ftaxon_id_ncbi.%20%7D%0A%20%20%20%20%7B%0A%20%20%20%20%20%20%3Fstatement%20prov%3AwasDerivedFrom%20%3Fref.%0A%20%20%20%20%20%20%3Fref%20pr%3AP248%20%3Freference.%0A%20%20%20%20%20%20%3Freference%20wdt%3AP356%20%3Freference_doi%3B%0A%20%20%20%20%20%20%20%20wdt%3AP1476%20%3Freference_title.%0A%20%20%20%20%7D%0A%20%20%7D%0A%20%20SERVICE%20wikibase%3Alabel%20%7B%20bd%3AserviceParam%20wikibase%3Alanguage%20%22%5BAUTO_LANGUAGE%5D%2Cen%22.%20%7D%0A%7D"></iframe>
        </p>
        </div>
        </div>
    </div>
<script src="https://ajax.googleapis.com/ajax/libs/jquery/3.2.1/jquery.min.js"></script>


<div class="container">
<div id="one-tab-content">
    <h5 class="title is-5" style="text-align:center;"> Composés reportés dans le genre Satureja </h5>
    <div class="columns is-centered" <p style="text-align: center">
    <iframe width=100% height="600" style="border:none;"
        src="https://query.wikidata.org/embed.html#SELECT%20DISTINCT%20%3Fcompound%20%3FcompoundLabel%20%3Finchikey%20%3Finchi%20%3Fsmiles_isomeric%20%3Fsmiles_canonical%20%3Fcas%20%3Fchebi%20%3Fchembl%20%3Fpubchem%20%3Ftaxon%20%3Ftaxon_name%20%3Ftaxon_id_gbif%20%3Ftaxon_id_ncbi%20%3Freference%20%3Freference_doi%20%3Freference_title%20WHERE%20%7B%0A%20%20%3Ftaxon%20wdt%3AP171%20%3Fparent_taxon.%0A%20%20%3Fparent_taxon%20wdt%3AP225%20%27Virola%27.%0A%20%20%3Fcompound%20wdt%3AP235%20%3Finchikey.%0A%20%20OPTIONAL%20%7B%20%3Fcompound%20wdt%3AP231%20%3Fcas.%20%7D%0A%20%20OPTIONAL%20%7B%20%3Fcompound%20wdt%3AP233%20%3Fsmiles_canonical.%20%7D%0A%20%20OPTIONAL%20%7B%20%3Fcompound%20wdt%3AP234%20%3Finchi.%20%7D%0A%20%20OPTIONAL%20%7B%20%3Fcompound%20wdt%3AP592%20%3Fchembl.%20%7D%0A%20%20OPTIONAL%20%7B%20%3Fcompound%20wdt%3AP662%20%3Fpubchem.%20%7D%0A%20%20OPTIONAL%20%7B%20%3Fcompound%20wdt%3AP683%20%3Fchebi.%20%7D%0A%20%20OPTIONAL%20%7B%20%3Fcompound%20wdt%3AP2017%20%3Fsmiles_isomeric.%20%7D%0A%20%20%7B%0A%20%20%20%20%3Fcompound%20p%3AP703%20%3Fstatement.%0A%20%20%20%20%3Fstatement%20ps%3AP703%20%3Ftaxon.%0A%20%20%20%20OPTIONAL%20%7B%20%3Ftaxon%20wdt%3AP225%20%3Ftaxon_name.%20%7D%0A%20%20%20%20OPTIONAL%20%7B%20%3Ftaxon%20wdt%3AP846%20%3Ftaxon_id_gbif.%20%7D%0A%20%20%20%20OPTIONAL%20%7B%20%3Ftaxon%20wdt%3AP685%20%3Ftaxon_id_ncbi.%20%7D%0A%20%20%20%20%7B%0A%20%20%20%20%20%20%3Fstatement%20prov%3AwasDerivedFrom%20%3Fref.%0A%20%20%20%20%20%20%3Fref%20pr%3AP248%20%3Freference.%0A%20%20%20%20%20%20%3Freference%20wdt%3AP356%20%3Freference_doi%3B%0A%20%20%20%20%20%20%20%20wdt%3AP1476%20%3Freference_title.%0A%20%20%20%20%7D%0A%20%20%7D%0A%20%20SERVICE%20wikibase%3Alabel%20%7B%20bd%3AserviceParam%20wikibase%3Alanguage%20%22%5BAUTO_LANGUAGE%5D%2Cen%22.%20%7D%0A%7D"></iframe>
    </p>
    </div>
</div>
</div>
<script src="https://ajax.googleapis.com/ajax/libs/jquery/3.2.1/jquery.min.js"></script>
