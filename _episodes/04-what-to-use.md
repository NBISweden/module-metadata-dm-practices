---
title: "How do I know what to use?"
teaching: 10
exercises: 20
questions:
- "?"
objectives:
- "To understand "
keypoints:
- ""
---

Given that reality is hard to categorise, and that different types of research investigate their subject matter from various different angles, there has emerged numerous different ontologies and metadata standards. In Life Science alone there are currently more than 800 standards. So how do I know what to use?

If you plan to deposit your data in a public repository (and you should) this is the first place to look for standards. They will have instructions for what metadata information they request for the data that they harbour. If you try to structure your own metadata according to these from the start, submitting your data will be a lot more straight-forward.

It is good practice to make a **data dictionary** for your metadata. This is a file that explains what type of information is supposed to be entered for at particular (meta)data field. This is where you document names of (meta)data fields, expected measurement units, allowed values, and definitions for what the field is about.

> ## Exercise: Start a data dictionary
>
> The file [FILE]() contains information about a set of samples for a research project. In this exercise you will start writing a data dictionary for this file.
> 1. Open the FILE that you downloaded in [lesson 1](01-what-is-the-problem), a spreadsheet program of you choice (Microsoft Excel, LibreOffice Calc, or Google Spreadsheet, or other).
> 2. Open another **empty** spreadsheet file, name it `data_dictionary`.
> 3. Add the following headings to the `data_dictionary` file:
> **Current variable name**, **Readable variable name**,	**ENA Variable name**,	**Measurement unit**,	**Allowed values**,	**Definition**,	**Description**
>
> 4. Copy the headings of the **FILE file** to the first column (Current variable name) of the `data_dictionary` file, _**one heading term per row**_.
>   * Now you should have a first row with the headings under step 3, and then one term (from the FILE file headings) per row in the first column.
> 5. Try adding definitions (to the Definition column) for some of the terms.
> 6. Are there any terms where you can specify information in the Measurement unit?
>
> > ## Solution
> >
> > The beginning av the data dictionary should look something like this:
> >
> > | Current variable name | Readable variable name | ENA Variable name | Measurement unit | Allowed values | Definition | Description |
> > |-|-|-|-|-|-|-|
> > | animal ID |  |  |  |  |  |  |
> > | date |  |  | YYYY-MM-DD |  |  |  |
> > | mouse line |  |  |  |  |  |  |
> > | strain |  |  |  |  | The mouse strain of the animal |  |
> > | age |  |  | days (?) |  | Age of animal |  |
> > | developmental stage |  |  |  |  |  |  |
> > | sex |  |  |  | male, female, unknown | Sex of the animal |  |
> > | organism part |  |  |  |  |  |  |
> > | genotype |  |  |  |  |  |  |
> > | experiment type |  |  |  |  |  |  |
> > | experiment reference |  |  |  |  |  |  |
> > | researcher |  |  |  |  |  |  |
> >
> {: .solution}
{: .challenge}


> ## Exercise: Look up an ENA checklist to improve the data dictionary
>
> Instruction instruction instruction…
{: .challenge}

> ## Solution
>
> * Do this
> * Do that
{: .solution}

Zooma

OLS

FAIRsharing.org is a resource that aims at collecting and connecting existing standards, databases. Use it to find recommended standards for different research domains and databases.


> ## Exercise: Find suitable ontologies for your data
>
> Instruction instruction instruction…
{: .challenge}

> ## Solution
>
> * Do this
> * Do that
{: .solution}