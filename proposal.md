This Google Season of Docs proposal was initially hosted at: https://gist.github.com/DrYak/ed38215519683ccd5c4657760050add7

# Better V-pipe tutorial for virus variant surveillance in wastewater

## Technical Writer Hiring

The V-pipe dev team is proud to be attributed a Google Season of Docs grant, and is happy to announce the partnership with ["van Geest Consultancy"](http://vangeestconsultancy.com/) for our tutorials writing project.

## About V-pipe

The [Computational Biology Group of ETH Zürich](https://bsse.ethz.ch/cbg) (CBG-ETHZ), [member of the Swiss Institute of Bioinformatics (SIB)](https://www.sib.swiss/niko-beerenwinkel-group), has developed the SIB Software Resource [V-pipe](https://github.com/cbg-ethz/V-pipe): an Apache-licensed computational pipeline for the analysis of virus next-generation sequencing (NGS) data, specializing in samples of mixed viral populations.

This bioinformatics workflow has important applications in several different settings:
- In clinical virology, information about the detection and quantification of viral quasispecies in a single patient sample can assist clinicians in the optimization of the treatment for this patient.
- In clinical epidemiology, sequencing test samples during a viral outbreak provides information about the viral variants found in the population, which helps better understanding of the epidemic dynamics and guiding the decision-making process of public health authorities in a timely fashion. 
- In environmental epidemiology, the sequencing of environmental samples enables the assessment of the circulation of viral variants independently of any large-scale public testing effort, but it requires specialized methods for deconvolution as a single sample provides information covering a large population of hosts living in that environment.

#### Role during the pandemic
  
In addition to its previous uses in clinical research settings such as HIV, our pipeline has thus seen increased use during the recent COVID-19 pandemic that started spreading into Europe in 2020, and V-pipe's automatic workflow played an important role in the genomic surveillance of SARS-CoV-2 in Switzerland (e.g.: the 75’000 sequences on [ENA](https://www.ebi.ac.uk/ena/browser/view/PRJEB43828) and GISAID published by the [Swiss SARS-CoV-2 sequencing consortium (S3C)](https://bsse.ethz.ch/cevo/research/sars-cov-2/swiss-sars-cov-2-sequencing-consortium.html) have been analyzed using our workflow).

#### Application to  wastewater

In particular, the analysis of environmental wastewater samples is an application for which the pipeline has been successfully adapted, based on its focus on analyzing mixtures of viral variants in a single sample: Such environmental surveillance of the SARS-CoV-2 pandemic has become an increasingly important source of information on the spread of variants since clinical tests declined and are currently close to disappearing. Our bioinformatics workflow V-pipe, including its components specialized in the analysis of wastewater, are at the core of the ongoing [wastewater-based SARS-CoV-2 variant monitoring](https://cov-spectrum.org/story/wastewater-in-switzerland) commissioned by the Swiss Federal Office of Public Health, a cornerstone of the current pandemic surveillance in Switzerland. These surveillance efforts enable early warning of the introduction of new variants, provides estimates of their spread, and evaluates epidemiological characteristics, earlier than traditional clinical surveillance and at a fraction of the cost ([10.1038/s41564-022-01185-x](https://doi.org/10.1038/s41564-022-01185-x), [10.1101/2022.11.02.22281825](https://doi.org/10.1101/2022.11.02.22281825), [10.4414/SMW.2022.w30202](https://doi.org/10.4414/SMW.2022.w30202)). 

#### V-pipe uses outside of Switzerland

Abroad, in the late 2021, a software component developed as part of the V-pipe bioinformatic workflow - the GPL-licensed COJAC - has been used by the UK Health Security Agency to monitor the spread of Omicron variant across 450 wastewater sampling sites in the UK ([Omicron, VOC- 21NOV-01 (B.1.1.529) Technical briefing 30](https://assets.publishing.service.gov.uk/government/uploads/system/uploads/attachment_data/file/1038404/Technical_Briefing_30.pdf)), a critical step in  understanding of the dynamics of the SARS-CoV-2 pandemic. More recently, in autumn 2023, V-pipe is being applied in a surveillance program in Northern Italy at Arpa Piemonte to help reduce the tedious work in searching for the variant BA.2.86 "_Pirola_" of SARS-CoV-2 in wastewater.

## The Problem

Given how Wastewater-based  epidemiology (WBE) is becoming critical in the face of declining clinical testing and sequencing, we would like to facilitate for other groups to replicate our viral variant surveillance bioinformatics data analysis. 
We are considering several strategies to enhance discoverability and ease of onboarding, including improved documentation. We are currently modernizing the website ([old version](https://web.archive.org/web/20240217110457/https://cbg-ethz.github.io/V-pipe/), [draft of new design](https://dryak.github.io/vpipe/)) and would like to take the opportunity to upgrade the documentations through the Google Season of Docs project.

The current state of the documentation:
- The `docs/` [subfolder of the project contains tutorials](https://github.com/cbg-ethz/V-pipe/tree/master/docs) for the installation and application of the workflow to HIV and SARS-CoV-2. That tutorial doesn't demonstrate the application on wastewater.
  -  these tutorials are also automatically executed as end-to-end test part of our CI using Jupytext.
- A [howto drafted demonstrating the analysis of wastewater](https://gist.github.com/DrYak/e28d5d523e644ea455748d540a32ad4d). This has been tested by researcher outside of our group working on separate wastewater analysis projects and confirmed working. It has also been the basis of a course at the University of Applied Sciences of the Grisons, yielding additional users feedback.
- A manual documenting the configuration file format is automatically generated in `config/config.html` based on the JSON schema (using [JSON Schema for Humans](https://github.com/coveooss/json-schema-for-humans))
- Additional information is spread between the [main readme file](https://github.com/cbg-ethz/V-pipe/blob/master/README.md) and the [config/README.md file](https://github.com/cbg-ethz/V-pipe/blob/master/config/README.md) (as required by [Standardized usage rules of the Snakemake Workflow Catalog](https://snakemake.github.io/snakemake-workflow-catalog/?rules=true)).

The SARS-CoV-2 tutorial need to be rewritten, incorporating the draft HOWTO on wastewater analysis. Also, the spread of information on multiple places causes potential users' confusion and hampers discoverability.

As a consequence of the current state of documentation, on-boarding new users has in the past required booking a video-conferencing call to brief interested new users, and walking them through the steps, which is not a long-term scalable solution.

## The Scope

### Main scope

The main scope of this project will consist of the following deliverable:

- Updated tutorial for SARS-CoV-2 covering the analysis of wastewater samples sequencing data.
  This is the minimum viable deliverable for the project.
- Expanded tutorial about the installation of V-pipe, with an added a "_Reusing an existing conda installation_" section.
- Organise these tutorial in the `docs/` folder, and write additional introduction, to make them available on the Read The Docs platform
- Review the main website and the README files to insure that information is properly linked, easily discoverable and reachable
  - Reduce duplication, while still fulfilling the mandatory requirements (e.g.:presence of file `config/README.md` is required by the Snakemake Workflow Catalog).

### Additional goals

Additional goals fitting within the scope if time permits:
- content of `config/config.html`  into the Read-The-Docs
- passing end-to-end CI test using the updated SARS-CoV-2 tutorial

### Out-of-scope for this project
- Recording an updated video presentation introducing this application of V-pipe will be dealt at a later point in time, outside this Google Season of Docs project.

## Measuring the results

### Internal measures
- Test the tutorial by sending to users with no prior experience analyze this type of data: 
  - ask members of the SIB to follow the tutorial and answer a short survey
  - new users at external partner centers replicating our methods (the current person working in Davos is defending his PhD soon and will need then to train a replacement)
- Test discoverability of information by giving exercise (again asking members of the SIB) in the form of: "_Use V-pipe to analyse this dataset..._"

### External measures
- the next 5 new centers interested in replicating our method should be able to do so without booking a video-conference call with the developer of V-pipe
- students at the next course using V-pipe should be able to complete tasks without opening issues on V-pipe

## Timeline
The project itself will take approximately four months to complete. The period after that will be used to track the performance of the updated documentation (see _External measures_ above).
Once the tech writer is hired, we'll spend two week on tech writer orientation (and familiarization with the technologies specific to our needs and pipeline: conda, jupytext, etc.), then move onto the inventory of existing documentation and tutorials, and definition of the content required to set up a proper Read The Docs documentation (two more weeks), and finally work the last three months on creating the defined content and populating it to the documentation (through an iterative process in collaboration with the pipeline developers).

Note: Timeline updated to match availability of technical writer.

| Dates       | Action Items                                                            |
| ----------- | ----------------------------------------------------------------------- |
| July        | -- Orientation and familiarization |
|             | -- Inventory of existing tutorials and documentation |
|             | -- Review proposed content to produce |
|             | -- Inventory of existing training material and proposed content to produce |
| August      | -- Create all identified content |
|             | -- Setup a Read the Doc |
|             | -- Populate branch of repository |
| Semptemer   | -- Review of contributions made to the documentation |
|             | -- Final changes requested by project members |
|             | -- Merge the updated docs/ and README into master |
|             | -- Linking documentation into website |
|             | -- Start to advertise the updated documentation |
| November    | -- Review the Measures |
|             | -- Project report |

## Project Budget

| Budget item      | Amount   |  Running Total | Notes/justifications |
| ---------------- | -------- | -------------- | -------------------- |
| Technical writer | $ 5,000  |  $ 5,000       | |
| Project swag     | $ 200    |  $ 5,200       | |
| **TOTAL**        |          |  **$ 5,200**   | |

---

## Changelog

2024-05-28 - Announcement of [Technical Writer](#technical-writer-hiring), Adjusting the [Timeline](#timeline) based on availability of van Geest Consultancy.
