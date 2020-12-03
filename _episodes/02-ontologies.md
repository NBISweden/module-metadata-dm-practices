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

Someone once said “A biologist would rather share a toothbrush with another biologist than share a gene name”. This is probably true for other domains of research too.  If we all stick to our own devices and name things as we see fit without regarding our fellow researchers we run the risk of being inconsistent and unclear. To help with consistency, we can use Controlled vocabularies or Ontologies when describing our data.

A **Controlled vocabulary** is a list of terms that describes a certain domain of knowledge. In the controlled vocabulary you only use one term to describe one particular phenomenon, excluding all other synonyms. The vocabulary should provide a _definition_ for the term, and any _synonyms_.

> ## How many terms for Breast Cancer can you think of?
>
> What would you...
>
> > ## Solution
> >
> > MeSH lists the following synonyms for “Breast Neoplasm”:
> >
> > - Breast Cancer
> > - Breast Carcinoma
> > - Breast Tumors
> > - Cancer of Breast
> > - Cancer of the Breast
> > - Human Mammary Carcinoma
> > - Malignant Neoplasm of Breast
> > - Malignant Tumor of Breast
> > - Mammary Cancer
> > - Mammary Carcinoma, Human
> > - Mammary Neoplasm, Human
> > - Mammary Neoplasms, Human
> > - Neoplasms, Breast
> > - Tumors, Breast
> {: .solution}
{: .challenge}

In a publicly managed controlled vocabulary, the terms should also have unique _identifiers_.

An **ontology** (in this context) is a controlled vocabulary, that appart from being a list of agreed terms, also captures relationships between these terms.

For example,

- in the [Human Phenotype Ontology](https://www.ebi.ac.uk/ols/ontologies/hp), **Myocardial infarction** is a _type_ of **Abnormal cardiovascular system physiology** is a _type_ of **Abnormality of the cardiovascular system** is a _type_ of **Phenotypic abnormality**.
- in the [BRENDA Tissue Ontology](https://www.ebi.ac.uk/ols/ontologies/bto), the **heart valve** is a _part_ of the **heart** is a _part_ of the **cardiovascular system** is a _part_ of the whole body.

As you see, depending on the way you look at reality, the domains of knowledge have to be structured in several different ways. There is no all-encompassing ontology that captures everything. You will have to rely on several different ontologies to describe your research. The question is which to choose.

You can decide to make your own controlled vocabularies. It might seem like less work than finding good ones that already exist. In the long run, you are better off using publicly managed vocabularies and lists, as much of the thinking about describing different domains has already been done. Another important aspects is that it will support the machine-readability aspect of FAIR. With unique identifiers for terms that describes your data (and their relationships), it can be possible for computer code to generate knowledge descriptions from data.
