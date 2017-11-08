<a id="top"></a>

* [About](#about)
* [Diagram](#diagram)
* [Examples](#examples)
* [Issues](#issues)

<a id="about"></a>
### About

Serves the vocabulary in JSON-LD at https://geodex.org/voc/

<a id="diagram"></a>
#### Diagram

![Research Repository Service Vocabulary](html/diagrams/diagram.png "Research Repository Service Vocabulary")

<a id="examples"></a>
#### Examples

All examples can be found at: https://github.com/earthcubearchitecture-project418/p418Vocabulary/blob/master/html/examples/

A [minimal record](https://github.com/earthcubearchitecture-project418/p418Vocabulary/blob/master/html/examples/required.jsonld) to satisfy the Research Repository Service:
```
{
    "@context": {
        "@vocab": "http://schema.org/",
        "gdx": "https://geodex.org/voc/"
    },
    "@type": "Service",
    "@id": "http://www.bco-dmo.org",
    "additionalType": "gdx:ResearchRepositoryService",
    "name": "Biological and Chemical Data Management Office Data Service",
    "url": "http://wwww.bco-dmo.org",
    "description": "The BCO-DMO resource catalog offers free and open access to publicly funded research products whose field of study are biological and chemical oceanography.",
    "provider": {
        "@type": "Organization",
        "@id": "http://www.bco-dmo.org/affiliation/191",
        "legalName": "Biological and Chemical Data Management Office",
        "url": "http://www.bco-dmo.org",
        "description": "The Biological and Chemical Oceanography Data Management Office (BCO-DMO) was created in late 2006 to serve PIs funded by the NSF Geosciences Directorate (GEO) Division of Ocean Sciences (OCE) Biological and Chemical Oceanography Programs and Office of Polar Programs (OPP) Antarctic Sciences (ANT) Organisms & Ecosystems Program. The BCO-DMO is a combination the Data Management Offices formerly created to support the US JGOFS and US GLOBEC programs. The BCO-DMO staff members are the curators of the legacy data collections created by those respective programs, as well as many other more recent research efforts including those of individual investigators.",
        "contactPoint": {
            "@id": "http:/www.bco-dmo.org/about-us",
            "@type": "ContactPoint",
            "name": "Support",
            "email": "info@bco-dmo.org",
            "url": "http:/www.bco-dmo.org/about-us",
            "contactType": "customer support"
        },
        "funder": {
            "@type": "Organization",
            "@id": "http://dx.doi.org/10.13039/100000141",
            "legalName": "Division of Ocean Sciences"
        }
    },
    "hasOfferCatalog": {
        "@type": "OfferCatalog",
        "additionalType": "gdx:ResearchResourceCatalog",
        "name": "BCO-DMO Resource Catalog",
        "itemListElement": [
            {
                "@type": "DataCatalog",
                "name": "BCO-DMO Data Catalog"
            }
        ]
    }
}
```

A [full record](https://github.com/earthcubearchitecture-project418/p418Vocabulary/blob/master/html/examples/full.jsonld):
```
{
    "@context": {
        "@vocab": "http://schema.org/",
        "gdx": "https://geodex.org/voc/"
    },
    "@type": "Service",
    "@id": "http://www.bco-dmo.org",
    "additionalType": "gdx:ResearchRepositoryService",
    "name": "Biological and Chemical Data Management Office Data Service",
    "url": "http://wwww.bco-dmo.org",
    "category": ["Biological Oceanography", "Chemical Oceanography"],
    "description": "The BCO-DMO resource catalog offers free and open access to publicly funded research products whose field of study are biological and chemical oceanography.",
    "sameAs": "http://www.re3data.org/repository/r3d100000012",
    "identifier": {
        "@type": "PropertyValue",
        "propertyID": "http://purl.org/spar/datacite/doi",
        "value": "10.17616/R37P4C",
        "url": "http://doi.org/10.17616/R37P4C"
    },
    "provider": {
        "@type": "Organization",
        "@id": "http://www.bco-dmo.org/affiliation/191",
        "identifier": "http://lod.bco-dmo.org/id/affiliation/191",
        "legalName": "Biological and Chemical Data Management Office",
        "name": "BCO-DMO",
        "url": "http://www.bco-dmo.org",
        "description": "The Biological and Chemical Oceanography Data Management Office (BCO-DMO) was created in late 2006 to serve PIs funded by the NSF Geosciences Directorate (GEO) Division of Ocean Sciences (OCE) Biological and Chemical Oceanography Programs and Office of Polar Programs (OPP) Antarctic Sciences (ANT) Organisms & Ecosystems Program. The BCO-DMO is a combination the Data Management Offices formerly created to support the US JGOFS and US GLOBEC programs. The BCO-DMO staff members are the curators of the legacy data collections created by those respective programs, as well as many other more recent research efforts including those of individual investigators.",
        "logo": {
            "@type": "ImageObject",
            "url": "http://www.bco-dmo.org/files/bcodmo/images/bco-dmo-words-BLUE.jpg"
        },
        "foundingDate": "2006-09-01",
        "address": {
            "@type": "PostalAddress",
            "streetAddress": "WHOI, MS#36, Shiverick House 11 School St.",
            "addressLocality": "Woods Hole",
            "addressRegion": "MA",
            "postalCode": "02543",
            "addressCountry": "USA"
        },
        "contactPoint": {
            "@id": "http:/www.bco-dmo.org/about-us",
            "@type": "ContactPoint",
            "name": "Support",
            "email": "info@bco-dmo.org",
            "url": "http:/www.bco-dmo.org/about-us",
            "contactType": "customer support"
        },
        "funder": {
            "@type": "Organization",
            "@id": "http://dx.doi.org/10.13039/100000141",
            "legalName": "Division of Ocean Sciences",
            "alternateName": "OCE",
            "url": "https://www.nsf.gov/div/index.jsp?div=OCE",
            "parentOrganization": {
                "@type": "Organization",
                "@id": "http://dx.doi.org/10.13039/100000085",
                "legalName": "Directorate for Geosciences",
                "alternateName": "NSF-GEO",
                "url": "http://www.nsf.gov",
                "parentOrganization": {
                    "@type": "Organization",
                    "@id": "http://dx.doi.org/10.13039/100000001",
                    "legalName": "National Science Foundation",
                    "alternateName": "NSF",
                    "url": "http://www.nsf.gov"
                }
            }
        },
        "parentOrganization": {
            "@type": "Organization",
            "@id": "http://www.whoi.edu",
            "name": "Woods Hole Oceanographic Institution",
            "url": "http://www.whoi.edu",
            "address": {
                "@type": "PostalAddress",
                "streetAddress": "266 Woods Hole Road",
                "addressLocality": "Woods Hole",
                "addressRegion": "MA",
                "postalCode": "02543",
                "addressCountry": "USA"
            }
        },
        "publishingPrinciples": [
            {
                "@type": "DigitalDocument",
                "additionalType": "gdx:Protocol-Access",
                "name": "Open Access Policy",
                "url": "http://www.bco-dmo.org/open-access-policy"
            },
            {
                "@type": "DigitalDocument",
                "additionalType": "gdx:Protocol-PreservationPolicy",
                "name": "Preservation Policy",
                "url": "http://www.bco-dmo.org/preservation-policy"
            }
        ]
    },
    "hasOfferCatalog": {
        "@type": "OfferCatalog",
        "additionalType": "gdx:ResearchResourceCatalog",
        "name": "BCO-DMO Resource Catalog",
        "itemListElement": [{
            "@type": "DataCatalog",
            "name": "BCO-DMO Data Catalog",
            "audience": {
                "@type": "Audience",
                "audienceType": "public",
                "name": "General Public"
            }
        }]
    },
    "availableChannel": [
        {
            "@type": "ServiceChannel",
            "additionalType": "gdx:SearchService",
            "name": "Website Search",
            "serviceUrl": "http://www.bco-dmo.org/search",
            "potentialAction": {
                "@type": "SearchAction",
                "target": {
                    "@type": "EntryPoint",
                    "contentType": "text/html",
                    "url": "http://www.bco-dmo.org/search",
                    "urlTemplate": "http://www.bco-dmo.org/search?keywords={query_string}",
                    "description": "Search the BCO-DMO catalog",
                    "httpMethod": "GET"
                }
            }
        },
        {
            "@type": "ServiceChannel",
            "additionalType": "gdx:SearchService",
            "name": "SPARQL Endpoint",
            "serviceUrl": "http://lod.bco-dmo.org/sparql",
            "potentialAction": {
                "@type": "SearchAction",
                "target": {
                    "@type": "EntryPoint",
                    "contentType": "application/sparql-query",
                    "url": "http://lod.bco-dmo.org/sparql",
                    "urlTemplate": "http://lod.bco-dmo.org/sparql?default-graph-uri={graph_iri}&query={query_string}&output={format}&timeout={timeout_sec}&debug={on_or_off}",
                    "description": "Search BCO-DMO RDF through its SPARQL Endpoint",
                    "httpMethod": ["GET", "POST"]
                }
            }
        },
        {
            "@type": "ServiceChannel",
            "additionalType": "gdx:SearchService",
            "name": "OAI-PMH Endpoint",
            "serviceUrl": "http://www.bco-dmo.org/services/oai",
            "potentialAction": {
                "@type": "SearchAction",
                "target": {
                    "@type": "EntryPoint",
                    "contentType": "application/xml",
                    "url": "http://www.bco-dmo.org/services/oai",
                    "urlTemplate": "http://www.bco-dmo.org/services/oai?verb={oai_verb}&metadataPrefix={metadata_format}",
                    "description": "Search BCO-DMO Datasets through its OAI-PMH Endpoint",
                    "httpMethod": "GET"
                }
            }
        },
        {
            "@type": "ServiceChannel",
            "additionalType": "gdx:SyndicationService",
            "availableLanguage": "en-US",
            "name": "RSS Feed of Recently Added Datasets",
            "url": "http://www.bco-dmo.org/how-get-started",
            "description": "Submit data to BCO-DMO",
            "serviceUrl": "http://www.bco-dmo.org/rss/datasets/recent.xml"
        },
        {
            "@type": "ServiceChannel",
            "additionalType": "gdx:SubmissionService",
            "availableLanguage": "en-US",
            "serviceUrl": "http://www.bco-dmo.org/how-get-started",
            "description": "Submit data to BCO-DMO"
        }
    ],
    "subjectOf": {
        "@type": "DigitalDocument",
        "additionalType": "gdx:SitemapXML",
        "name": "Sitemap XML for www.bco-dmo.org",
        "url": "https://www.bco-dmo.org/sitemap.xml",
        "description": "Listing of datasets and other resources available from the BCO-DMO data service"
    }
}
```

<a id="issues"></a>
#### Issues

https://stackoverflow.com/questions/38243521/schema-org-contacttype-validation-issue-the-value-provided-for-office-must-be

Back to [top](#top)
