---
title: "Controlled vocabularies & ontologies"
teaching: 10
exercises: 5
questions:
- "How can metadata be described consistently?"
objectives:
- "To understand what controlled vocabularies and ontologies are"
keypoints:
- "Use controlled vocabularies and ontologies when specifying metadata"
---

Someone once said “A biologist would rather share a toothbrush with another biologist than share a gene name”. This is probably true for other domains of research too.  If we all stick to our own devices and name things as we see fit without regarding our fellow researchers we run the risk of being inconsistent and unclear. To help with consistency when describing our data, we can use standardized term collections - Controlled vocabularies, Ontologies, Thesauruses, and Taxonomies. _The names for these different types of collections are often used interchangeably_.

> ## How many terms for Breast Cancer can you think of?
>
> Discuss with your neighbour about what other terms you could use for "Breast Cancer".
>
> > ## Solution
> >
> > MeSH lists the following synonyms for “Breast Neoplasm”:
> >
> > - Breast Neoplasm
> > - Neoplasm, Breast
> > - Breast Tumors
> > - Breast Tumor
> > - Tumor, Breast
> > - Tumors, Breast
> > - Neoplasms, Breast
> > - Breast Cancer
> > - Cancer, Breast
> > - Mammary Cancer
> > - Cancer, Mammary
> > - Cancers, Mammary
> > - Mammary Cancers
> > - Malignant Neoplasm of Breast
> > - Breast Malignant Neoplasm
> > - Breast Malignant Neoplasms
> > - Malignant Tumor of Breast
> > - Breast Malignant Tumor
> > - Breast Malignant Tumors
> > - Cancer of Breast
> > - Cancer of the Breast
> > - Mammary Carcinoma, Human
> > - Carcinoma, Human Mammary
> > - Carcinomas, Human Mammary
> > - Human Mammary Carcinomas
> > - Mammary Carcinomas, Human
> > - Human Mammary Carcinoma
> > - Mammary Neoplasms, Human
> > - Human Mammary Neoplasm
> > - Human Mammary Neoplasms
> > - Neoplasm, Human Mammary
> > - Neoplasms, Human Mammary
> > - Mammary Neoplasm, Human
> > - Breast Carcinoma
> > - Breast Carcinomas
> > - Carcinoma, Breast
> > - Carcinomas, Breast
> {: .solution}
{: .challenge}

A **Controlled vocabulary** is a list of terms that describes a certain domain of knowledge. In the controlled vocabulary you only use _one_ term to describe one particular phenomenon, excluding all other synonyms. The vocabulary should provide a _definition_ for the term, and any _synonyms_. In a publicly managed controlled vocabulary, the terms should also have unique _identifiers_, so that they can be referenced.

An **ontology** (in this context) is a controlled vocabulary, that apart from being a list of agreed terms, also captures relationships between these terms.

For example,

- in the [Human Phenotype Ontology](https://www.ebi.ac.uk/ols/ontologies/hp), **Myocardial infarction** is a _type_ of **Abnormal cardiovascular system physiology** is a _type_ of **Abnormality of the cardiovascular system** is a _type_ of **Phenotypic abnormality**.
- in the [BRENDA Tissue Ontology](https://www.ebi.ac.uk/ols/ontologies/bto), the **heart valve** is a _part_ of the **heart** is a _part_ of the **cardiovascular system** is a _part_ of the whole body.

As you see, depending on the way you look at reality, the domains of knowledge have to be structured in several different ways. There is no all-encompassing ontology that captures everything. You will have to rely on several different ontologies to describe your research. The question is which to choose.

You can decide to make your own controlled vocabularies. It might seem like less work than finding good ones that already exist. In the long run, you are better off using publicly managed vocabularies and lists, as much of the thinking about describing different domains has already been done. Another important aspects is that it will support the machine-readability aspect of FAIR. With unique identifiers for terms that describes your data (and their relationships), it can be possible for computer code to generate knowledge descriptions from data.
