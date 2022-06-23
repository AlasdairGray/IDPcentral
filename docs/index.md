---
layout: default

bioschemas:
  "@context": https://schema.org
  "@type": DataCatalog
  "http://purl.org/dc/terms/conformsTo":
  - "@type": CreativeWork
    "@id": "https://bioschemas.org/profiles/DataCatalog/0.3-RELEASE-2019_07_01"
  "description": "Knowledge graph about Intrinsically Disordered Proteins generated from Bioschemas markup embedded within DisProt, MobiDB, and ProteinEnsemble."
  "keywords": "IDP, Protein"
  "license": "https://creativecommons.org/share-your-work/public-domain/cc0/"
  "name": "Intrinsically Disordered Proteins Knowledge Graph (IDP-KG)"
  "url": "https://alasdairgray.github.io/IDP-KG/"
  "provider":
  - "@type": Person
    name: "Alasdair Gray"
    "@id": http://orcid.org/0000-0002-5711-4872
    "url": http://orcid.org/0000-0002-5711-4872
  - "@type": Person
    name: "Petros Papadopoulos"
    "@id": https://orcid.org/0000-0002-8110-7576
    url: https://orcid.org/0000-0002-8110-7576
  - "@type": Person
    name: "Imran Asif"
    "@id": https://orcid.org/0000-0002-1144-6265
    url: https://orcid.org/0000-0002-1144-6265
  - "@type": Person
    name: "Ivan Mi&ccaron;eti&cacute;"
    "@id": https://orcid.org/0000-0003-1691-8425
    url: https://orcid.org/0000-0003-1691-8425
  - "@type": Person
    name: "Andras Hatos"
    "@id": https://orcid.org/0000-0001-9224-9820
    url: https://orcid.org/0000-0001-9224-9820
  "dataset":
  - "@type": Dataset
    "@id": https://alasdairgray.github.io/IDP-KG/versions/idp-kg_2021-09-07
  - "@type": Dataset
    "@id": https://alasdairgray.github.io/IDP-KG/versions/idp-kg_2021-09-28
---

# IDP-KG

The Intrinsically Disordered Protein Knowledge Graph (IDP-KG) supports the discovery of information about proteins that are known to be disordered. It has been generated from the [Bioschemas](https://bioschemas.org) markup deployed on three data sources from the [ELIXIR Intrinsically Disordered Protein Community](https://elixir-europe.org/communities/intrinsically-disordered-proteins). The data sources that are aggregated are:
- [DisProt](https://disprot.org)
- [MobiDB](https://mobidb.org)
- [Protein Ensemble (PED)](https://proteinensemble.org)

## IDP-KG Versions

The following versions of the IDP-KG are available:
- [IDP-KG_2022-06-21](versions/idp-kg_2022-06-21)
- [IDP-KG_2021-09-28](versions/idp-kg_2021-09-28)
- [IDP-KG_2021-09-07](versions/idp-kg_2021-09-07)

## Funding and Acknowledgements

<img style="float: right;" src="https://bioschemas.org/images/Elixir-logo.png" alt="ELIXIR Logo">

This work was funded as part of the [ELIXIR Interoperability Platform](https://www.elixir-europe.org/services/interoperability/) Strategic Implementation Study [_"Bioschemas Markup to Support ELIXIR Communities"_](https://elixir-europe.org/about-us/commissioned-services/exploiting-bioschemas-markup-support-elixir-communities).

Early stages of this work were carried out during the [BioHackathon Europe 2020](https://2020.biohackathon-europe.org/) organized by [ELIXIR](https://elixir-europe.org/) in November 2020. We thank the organizers and fellow participants for their discussions and contributions.

<!-- Embed Bioschemas Markup  -->
{% if page.bioschemas %}
  <script type="application/ld+json">
     {{ page.bioschemas | jsonify }}
  </script>
{% endif %}
