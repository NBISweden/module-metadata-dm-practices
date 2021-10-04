---
title: "Data dictionary"
teaching: 5
exercises: 20
questions:
- "How do to document the standards to use?"
objectives:
- "To understand how to document the standards and conventions to use for my data"
keypoints:
- "Use data dictionaries to document standards for your data"
---

It is good practice to make a **data dictionary** for your metadata. This is a file that explains what type of information is supposed to be entered for at particular (meta)data field. This is where you document names of (meta)data fields, expected measurement units, allowed values, and definitions for what the field is about.

> ## Exercise: Start a data dictionary
>
> The file [samples_metadata_lesson.csv](../files/samples_metadata_lesson.csv) contains information about a set of samples for a research project. In this exercise you will start writing a data dictionary for this file.
> 1. Open the `samples_metadata_lesson.csv` file in a spreadsheet program of you choice (Microsoft Excel, LibreOffice Calc, or Google Spreadsheet, or other).
> 2. Open another **empty** spreadsheet file, name it `data_dictionary`.
> 3. Add the following headings to the `data_dictionary` file:
> **Current variable name**, **ENA Variable name**, **Measurement unit**, **Allowed values**, **Definition**, **Description**
>
> 4. Copy the headings of the **FILE file** to the first column (Current variable name) of the `data_dictionary` file, _**one heading term per row**_.
>   * Now you should have a first row with the headings under step 3, and then one term (from the FILE file headings) per row in the first column.
> 5. Try adding definitions (to the Definition column) for some of the terms.
> 6. Are there any terms where you can specify information in the Measurement unit?
>
> > ## Solution
> >
> > The beginning of the data dictionary could now look something like this:
> >
> > | Current variable name | ENA Variable name | Measurement unit | Allowed values | Definition | Description |
> > |-|-|-|-|-|-|
> > | sample id |  |  |  |  |  |
> > | patient id |  |  |  |  |  |
> > | sex |  |  | male, female, unknown | Sex of the individual |  |
> > | date |  |  | format: YYYY-MM-DD, >=proj_start_date & <=today | Date of sampling |  |
> > | location |  |  |  |  |  |
> > | age |  | years |  | Age of individual at the time of sampling |  |
> > | health state |  |  |  | Health state of individual at time of sampling |  |
> > | symptoms |  |  | fever, sore throat, fatigue, loss of taste, not applicable | Symptoms experienced in connection with illness |  |
> > | disease outcome |  |  | healthy, dead | Final outcome of disease |  |
> > | tissue |  |  |  | Tissue sampled |  |
> >
> {: .solution}
{: .challenge}

If you plan to deposit your data in a public repository (and you should) this is the first place to look for standards. They will have instructions for what metadata information they request for the data that they harbour. If you try to structure your own metadata according to these from the start, submitting your data will be a lot more straight-forward.

> ## Exercise: Look up an ENA checklist to improve the data dictionary
>
> In this exercise we are assuming that you are planning to submit data about your samples to the European Nucleotide Archive - ENA. The ENA has sets of suggested metadata standards for different types of samples that they call checklists.
> 1. Go to [https://www.ebi.ac.uk/ena/browser/checklists](https://www.ebi.ac.uk/ena/browser/checklists) to see the available checklists
> 2. Scroll down the listing until you find the *ERC000033 ENA virus pathogen reporting standard checklist*
> 3. The _ENA virus pathogen reporting standard checklist_ lists the expected name and content for a number of metadata fields that can be submitted for samples. If you put your mouse pointer over the ? icon, you will get a description about of what type of information the different fields are supposed to contain.
> 4. Open the **data dictionary file** that you started in the previous exercise.
> 5. Go through the data dictionary and find suitable field names in the _ENA virus pathogen reporting standard checklist_ for those fields. Add them to the **ENA Variable name column** of your data dictionary file. 
>   - Are all mandatory fields present, or will you need to add fields?
>   - Are there fields that need to be split into more fields?
> 6. Also, note if any of the fields have controlled vocabularies. Update the allowed values for those fields in the data dictionary.
>
> > ## Solution
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
> > | symptoms | **illness symptoms** |  | fever, sore throat, fatigue, loss of taste or smell, not applicable | Symptoms experienced in connection with illness |  |
> > | disease outcome | **host disease outcome** |  | **recovered**, dead | Final outcome of disease |  |
> > | tissue | **isolation source host-associated** |  |  | Tissue sampled |  |
> > | **isolate** | **isolate** |  |  | **individual isolate from which the sample was obtained** |  |
> >
> {: .solution}
{: .challenge}
