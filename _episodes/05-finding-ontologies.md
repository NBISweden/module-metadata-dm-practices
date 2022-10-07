---
title: "Finding ontologies"
teaching: 10
exercises: 20
questions:
- "How can I find suitable ontologies to describe my data?"
objectives:
- "To be aquainted with some different examples of how to find ontologies and ontology terms"
keypoints:
- "There are tools and resources available to find standards and ontologies"
- "It is not always straightforward to find standards and ontologies"
---

As you noticed in the previous excercise, the ENA checklist did not specify any particular standard to use when assigning values to the different fields. However, if you can be more specific regarding how you describe the different metadata aspects for your data it will increase the FAIRness of your data. For this you should use controlled vocabularies or ontologies.

As we have said earlier, there are hundreds of metadata standards, controlled vocabularies and ontologies in the Life Sciences alone. So how do you find the ones that are appropriate for your data? Fortunately, there are tools and resources to help you with this.

[FAIRsharing.org](https://fairsharing.org) is a resource that aims at collecting and connecting existing standards and databases. Use it to find recommended standards for different research domains and databases.

The [European Bioinformatics Institute (EMBL-EBI)](https://www.ebi.ac.uk/) makes availble a [set of resources for ontologies](https://www.ebi.ac.uk/spot/ontology/), e.g.:

* [OLS](https://www.ebi.ac.uk/ols/index)
* [Zooma](https://www.ebi.ac.uk/spot/zooma/)

> ## Exercise: Find suitable ontologies for your data
>
> To be more specific about the terms used for some of the fields, try to find a suitable ontology and the terms to use for the values that will be in your data file ([samples_metadata_lesson.csv](../files/samples_metadata_lesson.csv)), for these fields:
> * **illness symptoms**, using OLS
> * **isolation source host-associated**, using FAIRsharing.org
>
> Add the name of the ontology and the terms you have selected to the **data dictionary**.
>
> You don't have to stick to the tools specified. Try different ones if you want to. As you will probably notice, there is no perfect way that always finds what you want. It will almost always involve a fair bit of trial and error.
>
> > ## Solution
> >
> > * For each field you will have to look into the data file to see what values are there now
> > * Then try to find an ontology and the appropriate terms in that ontology
> > * Add the name of the ontology and the terms you have choosen to the allowed values columns
> >
> > **illness symptoms**
> > * Go to OLS, search for one of the symptoms in the `samples_metadata_lesson.csv` file, e.g. _fever_
> > * Choose one of the search results that seems appropriate, e.g. from the _NCI Thesaurus OBO Edition - **NCIT**_
> > * The term for _fever_ in NCIT is **Fever**. Also note that it has an identifier _NCIT:C3038_
> > * Find terms for the other symptoms in NCIT, by either browsing the tree (click on the Show siblings button in the ontology tree to expand the contents of the tree), or by searching
> > * See below for the NCIT terms for the symptoms
> >
> > **isolation source host-associated**
> > * Go to FAIRsharing.org
> > * Click STANDARDS at the top of the page
> > * Search for "anatomy" on the left hand side of the page
> > * Find a suitable ontology, e.g. _Foundational Model of Anatomy - **FMA**_, and go to the information page
> > * Scroll down to the ADDITIONAL INFORMATION section at the bottom, and click the link to _BioPortal_
> > * Select the classes tab. Look through the tree of terms, or search for a term in the "Jump to" field
> > * So **FMA** would be a suitable ontology. See below for the FMA terms for the tissues
> >
> > The data dictionary could now look something like this:
> >
> > | Current variable name | ENA Variable name | Measurement unit | Allowed values | Definition | Description |
> > |-|-|-|-|-|-|
> > | sample id |  |  |  |  |  |
> > | patient id | **host subject id** |  |  |  |  |
> > | sex | **host sex** |  | male, female, **not collected** | Sex of the individual |  |
> > | date | **collection date** |  | format: YYYY-MM-DD, >=proj_start_date & <=today | Date of sampling |  |
> > | location | **geographic location (country and/or sea)** |  | <country> |  |  |
> > | location | **geographic location (region and locality)** |  | <region>, <city>, ... |  |  |
> > | age | **host age** | years |  | Age of individual at the time of sampling |  |
> > | health state | **host health state** |  | **diseased, healthy, not applicable, not collected, not provided, restricted access** | Health state of individual at time of sampling |  |
> > | symptoms | **illness symptoms** |  | **NCIT ontology: <br>Fever (NCIT:C3038), Sore Throat (NCIT:C50747), Fatigue (NCIT:C3036), Ageusia (NCIT:C116374), not applicable** | Symptoms experienced in connection with illness |  |
> > | disease outcome | **host disease outcome** |  | **recovered**, dead | Final outcome of disease |  |
> > | tissue | **isolation source host-associated** |  | **FMA ontology:<br>Laryngopharynx (FMA:54880), Nasopharynx (FMA:54878), Lung (FMA:7195)** | Tissue sampled |  |
> > | **isolate** | **isolate** |  |  | **individual isolate from which the sample was obtained** |  |
> >
> {: .solution}
{: .challenge}

Below are list for some commonly used ontologies. Please note that this is in no way an exhaustive or a "standard" list.

### "Upper ontologies"

* [Semanticscience Integrated Ontology, SIO](https://bioportal.bioontology.org/ontologies/SIO)
* [Basic Formal Ontology, BFO](https://bioportal.bioontology.org/ontologies/BFO)
* [Relations Ontology](https://bioportal.bioontology.org/ontologies/OBOREL)
* [The Dublin Core (DC) Ontology](http://dublincore.org/)


### "Domain ontologies"

* [Gene Ontology, GO ](http://www.geneontology.org/)
* [Gene Ontology Annotation, GOA](http://www.ebi.ac.uk/GOA/)
* [Experimental Factor Ontology, EFO](https://bioportal.bioontology.org/ontologies/EFO)
* [The Environment Ontology, ENVO](http://environmentontology.org)
* [Mondo Disease Ontology](https://mondo.monarchinitiative.org)
* [uPheno Ontology](https://github.com/obophenotype/upheno)
* [The Human Phenotype Ontology](https://hpo.jax.org/app/)


### "Other ontologies"

* [The Friend Of A Friend (FOAF) ontology]( http://www.foaf-project.org/)
* [Research Object Ontology, RDO](https://www.researchobject.org/initiative/research-object-model/)
* [Data Catalogue Vocabulary, DCAT](https://www.w3.org/TR/vocab-dcat-3/)
* [Provenance Ontology, PROV-O](https://www.w3.org/TR/prov-o/)
* [Data Use Ontology](https://github.com/EBISPOT/DUO)
