<a id="top"></a>

* [About](#about)
* [Diagrams](#diagrams)
  * [Repository](#repository-diagram)
  * [Dataset](#dataset-diagram)
    * [Variables](#dataset-variables)
    * [Spatial](#dataset-spatial)
    * [Temporal](#dataset-temporal)
    * [Identifiers](#dataset-identifiers)
    * [Creators/Contributors](#dataset-creator_contributor)
    * [Publisher/Provider](#dataset-publisher_provider)
    * [Distributions](#dataset-distros)
    * [Protocols](#dataset-protocols)
    * [Funding](#dataset-funding)
    * [Deployment]($dataset-deployment)
    * [Project](#dataset-project)
    * [DataCatalog](#dataset-catalog)
  * [Graphical Notation](#graphical-notation)
* [Examples](#examples)
* [Issues](#issues)

<a id="about"></a>
## About

Serves the vocabulary in JSON-LD at https://geodex.org/voc/.

## Goals

1) To produce quality schema.org markup with additional extensions to schema.org classes to help improve harvesting technologies.

2) Produced markup will pass the [Google Structured Data Testing Tool](https://search.google.com/structured-data/testing-tool/u/0/) with 0 errors.

## Approach

To produce quality schema.org, all extensions to schema.org classes will be made through the use of the recommended property [schema:additionalType](https://schema.org/additionalType). The gdx: vocabulary will extend schema.org using rdfs:subClassOf in it's formal ontology, but in schema.org this doesn't translate into the use of JSON-LD's [@type](https://www.w3.org/TR/json-ld/#syntax-tokens-and-keywords) as traditional RDF publishing would encourage.

### Prefix

| Prefix        | Vocabulary URI |
| ------------- |----------------|
| schema:       | [<https://schema.org/>](https://schema.org/) |
| gdx:          | [<https://geodex.org/voc/>](https://geodex.org/voc/) |
| earthcollab:  | [<https://library.ucar.edu/earthcollab/schema#>](https://library.ucar.edu/earthcollab/schema#) |
| geolink:      | [<http://schema.geolink.org/1.0/base/main#>](http://schema.geolink.org/1.0/base/main#) |
| vivo:         | [<http://vivoweb.org/ontology/core#>](http://vivoweb.org/ontology/core#) |
| geo-upper:    | [<http://www.geoscienceontology.org/geo-upper#>](http://www.geoscienceontology.org/geo-upper#) |
| dbpedia:      | [<http://dbpedia.org/resource/>](http://dbpedia.org/resource/) |
 
schema: the defacto vocabulary for publishing structured data in web pages for search engine harvesting
gdx: the P418 project's vocabulary
earthcollab: an EarthCube Building Block focusing on extensions to the ViVO ontology
vivo: the ViVO ontology
geo-upper: a segment of the Geoscience Standard Names Ontology, an EarthCube product
dbpedia: Structured data for Wikipedia resources

<a id="repository-diagram"></a>
### Publishing metadata about a Repository

Because the organizational and governance structures of all repositories vary, this vocabulary has split apart the *function* of the repository from the organization(s) that operate/provide those functions. In schema.org, this *function* is best described as a [schema:Service](https://schema.org/Service), and to uniquely identify repositories curating research products, this vocabulary defines an extension to schema:Service as [gdx:ResearchRepositoryService](https://geodex.org/voc/ResearchRepositoryService).

![Research Repository Service Vocabulary](https://cdn.rawgit.com/earthcubearchitecture-project418/p418Vocabulary/master/html/voc/static/schema/diagrams/repository.svg "Research Repository Service")


<a id="dataset-diagram"></a>
### Dataset
![Dataset](html/voc/static/schema/diagrams/dataset.png "Dataset")

<a id="dataset-variables"></a>
#### Variables
![Variables](html/voc/static/schema/diagrams/dataset-variables.png "Dataset - Variables")


<a id="dataset-spatial"></a>
#### Spatial
![Spatial](html/voc/static/schema/diagrams/dataset-spatial.png "Dataset - Spatial")


<a id="dataset-temporal"></a>
#### Temporal
![Temporal](html/voc/static/schema/diagrams/dataset-temporal.png "Dataset - Temporal")


<a id="dataset-identifiers"></a>
#### Identifiers
![Identifiers](html/voc/static/schema/diagrams/dataset-identifier.png "Dataset - Identifiers")


<a id="dataset-creator_contributor"></a>
#### Creators/Contributors
![Variables](html/voc/static/schema/diagrams/dataset-variables.png "Dataset - Variables")


<a id="dataset-publisher_provider"></a>
#### Publisher/Provider
![Publisher/Provider](html/voc/static/schema/diagrams/dataset-publisher_provider.png "Dataset - Publisher/Provider")


<a id="dataset-distros"></a>
#### Distributions
![Distributions](html/voc/static/schema/diagrams/dataset-distribution.png "Dataset - Distributions")


<a id="dataset-protocols"></a>
#### Protocols
![Protocols](html/voc/static/schema/diagrams/dataset-protocols.png "Dataset - Protocols")


<a id="dataset-funding"></a>
#### Funding
![Funding](html/voc/static/schema/diagrams/dataset-funding.png "Dataset - Funding")


<a id="dataset-deployment"></a>
#### Deployment
![Deployment](html/voc/static/schema/diagrams/dataset-deployment.png "Dataset - Deployment")


<a id="dataset-project"></a>
#### Project
![Project](html/voc/static/schema/diagrams/dataset-project.png "Dataset - Project")


<a id="dataset-catalog"></a>
#### DataCatalog
![DataCatalog](html/voc/static/schema/diagrams/dataset-catalog.png "Dataset - Catalog")


<a id="graphical-notation"></a>
#### Graphical Notation
![Graphical Notation](html/voc/static/schema/diagrams/graphical-notation.png "Graphical Notation")

Back to [top](#top)

<a id="examples"></a>
### Examples

All examples can be found at: https://github.com/earthcubearchitecture-project418/p418Vocabulary/blob/master/html/examples/

A [minimal record](https://github.com/earthcubearchitecture-project418/p418Vocabulary/blob/master/html/examples/required.jsonld) to satisfy the Research Repository Service.

A [full record](https://github.com/earthcubearchitecture-project418/p418Vocabulary/blob/master/html/examples/full.jsonld).

<a id="issues"></a>
#### Issues

https://stackoverflow.com/questions/38243521/schema-org-contacttype-validation-issue-the-value-provided-for-office-must-be

Back to [top](#top)
