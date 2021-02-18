---
title: "Metadata standards"
teaching: 10
exercises: 0
questions:
- "What are metadata standards?"
objectives:
- "To understand what a metadata standard is"
keypoints:
- "There are generic and domain-specific standards"
---

A metadata standard could be described as a collection of metadata fields or elements that are of relevance for the particular type of scientific study data that is to be documented. Such standards will often consist of some elements that are mandatory, some recommended, and some that are optional. They will (at least should) define what type of input values are expected for each element, e.g. free text, date in a specific format, geographical positions, numerical values, and controlled vocabularies or ontologies. Sometimes the element name itself is a specified ontology term. The further we go on being strict about defining the elements and values the more we open up for increasing the FAIRness aspects of the data from a computational point of view.

Standards range from the very generic to the very specific. Let’s have a look at a couple of examples:

* The [Dublin Core](https://www.dublincore.org/specifications/dublin-core/dces/) is a generic standard for describing digital and physical resources. In its basic form it specifies 15 elements, such as Creator, Title, Description, Date, etc.

* An example of a more specific standard is the [ENA virus pathogen reporting standard checklist](https://www.ebi.ac.uk/ena/browser/view/ERC000033), for reporting metadata of virus pathogen samples associated with genomic data to the European Nucleotide Archive. It has 35 elements, of which 9 are mandatory and 15 recommended. Example of elements are geographic location, host scientific name, host health state, collection date, etc.

Given that reality is hard to categorise, and that different types of research investigate their subject matter from various different angles, there has emerged numerous different ontologies and metadata standards. In Life Science alone there are currently more than 800 standards. So how do I know what to use?
