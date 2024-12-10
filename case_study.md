# Google Season of Docs Case Study Template


# V-pipe: 2024 Google Season of Docs Case Study

**Organization / Project Name:**  
V-pipe \- Better V-pipe tutorial for virus variant surveillance in wastewater

**Season of Docs link:**  
[https://gist.github.com/DrYak/ed38215519683ccd5c4657760050add7](https://gist.github.com/DrYak/ed38215519683ccd5c4657760050add7) 

**Organization Description:**  

V-pipe is an open-source (Apache) computational pipeline for analysis of virus next-generation sequencing (NGS) data, specialized in samples of mixed viral population origin.

A key application of V-pipe is its use in the ongoing wastewater-based SARS-CoV-2 variant monitoring commissioned by the Swiss Government. These surveillance efforts enable early warning of the occurrence of new virus variants, by providing estimates of their spread, and an evaluation of the epidemiological characteristics of the new virus variant. This application is faster than traditional clinical surveillance and additionally, only  a fraction of the costs compared to traditional clinical surveillance is needed.

**Authors:**   
- [Ivan Topolsky](https://github.com/DrYak) \- Computational Biology Group ETH Zürich, Project submitter  
- [Geert van Geest](https://github.com/GeertvanGeest) \- van Geest Consultancy, Technical writer  
- [PD Dr. Katja Baerenfaller](https://www.siaf.uzh.ch/molecular_allergology_katja.html) \- Group leader at SIAF, University of Zurich, teaches at the University of Applied Sciences of the Grisons.  
- [Niko Beerenwinkel](https://bsse.ethz.ch/cbg) \- Group leader of Computation Biology Group ETH Zürich

## Summary

| \# Tech Writers | TW Project Hours | Budget | % Project Completed |
| :---: | :---: | :---: | :---: |
| 1 | 40 | $5000 | 100% |

**What problem were you trying to solve? And how did you try to solve it?**

Our goal was to simplify the onboarding of new users interested in replicating the kind of wastewater-based surveillance of viral variants of SARS-CoV-2 that we do nationally in Switzerland.

Our technical writer updated and reorganized the documentation, wrote a new tutorial specific to the analysis of sequencing data of such wastewater-based variants surveillance, and set up this documentation on Read the Docs.

**What were the outcomes of your project?**

We now have a new modernized documentation available in a format published on Read the Docs.
This new documentation makes it simpler for new users start similar analyses: students successfully tested it during assignments where they were tasked with performing such analyses of wastewater-based surveillance sequencing data.

**What went well? And what would you do differently?**

We are very happy with the whole writing process and the new documentation.
The hiring process turned out more complex than expected.

**What advice would you give to other projects trying to solve a similar problem with documentation?**

Use user feedback to identify points of improvement in the documentation.
Ideally set up controlled environment for testing the documentations (e.g.: students assignments, reproducibility hackathons).
Plan clear tasks leading to specific deliverables.
Leverage you network to find a technical writer in advance.


## Project Description

### Project Proposal

V-pipe is an open-source (Apache) computational pipeline for the analysis of virus next-generation sequencing (NGS) data, specialized in samples of mixed viral population origin.

The application is very versatile and modular. However, its configurability can seem daunting for beginning users.

To facilitate the onboarding of new users interested in replicating the kind of wastewater-based surveillance of viral variants of SARS-CoV-2 that we do nationally, we are updating our documentation. We will write a new tutorial demonstrating this specific application of V-pipe. Additionally, we will reorganize existing documentation and set up an online accessible documentation on Read the Docs.

Full proposal at this link:  
[https://gist.github.com/DrYak/ed38215519683ccd5c4657760050add7](https://gist.github.com/DrYak/ed38215519683ccd5c4657760050add7) 

### Proposal Creation Process

*How did you come up with your Google Season of Docs proposal? What process did your organization use to decide on an idea? How did you solicit and incorporate feedback? Who participated in the process? How long did it take?*

We had reached the conclusion that to achieve significant improvement of the quality of documentation, we would need hiring an experienced professional writer. As Google Season of Docs provides grants to work on documentation for open-source software projects, we decided to submit a proposal.

For the proposal we selected a clearly defined main task. This task is writing a much-needed tutorial demonstrating a specific application of V-pipe in the context of wastewater analysis. We already have an internal draft that demonstrates the steps and we also have example datasets from past publications. The results from these publications can be reproduced as part of this tutorial. This makes the tasks clearly defined and helps the writer know where to start working from.

Additional tasks included restructuring the documentation, and integrating into our CI/CD processes. Our old tutorials were automatically executed as end-to-end tests for our pipeline.  We also need to integrate the exhaustive manual for the configuration file format that is automatically generated from V-pipe’s source code (from the validation json schemas). These tasks are quite specific to our development process. We kept them manageable by clearly defining the tasks and planning necessary onboarding time at the beginning of the project schedule. This allowes the writer to familiarize with the peculiarities of these tasks.

Although we did not seek much feedback for the specific proposal written for GSoD (i.e.: not for the text at the URL mentioned above), the tasks listed in the proposal were formed after gathering feed-back from users, students attending past workshops and lectures, and issues filed on GitHub. This helped us focus on the points most likely to help our users, and made selecting tasks for the GSoD proposal straightforward.

The writing of the GSoD proposal itself took place over a couple of weeks, but the selection of tasks comes from input gathered over the past two years since the initial full integration of all processing tools into the V-pipe workflow (as part of the Elixir BioHackthon Europe 2022 \- doi:[10.37044/osf.io/rtgk9](http://osf.io/rtgk9)).

### Budget

| How much money did you ask for?  | 5200 |
| :---- | :---- |
| How did you come up with this estimate? | We intentionally concentrated on a smaller clearly defined main task that could be worked within the entry-level budget proposed by GSoD. |
| How many hours of work did you budget for the project?  | 40 |
| How many hours of work were actually needed for the project? | 40 |
| What other expenses did you include in your budget? | 200 for goodies |
| Did you run into any budget surprises during the project (e.g. misestimates)? If so, please explain. | No. Task successfully led to completion, including extra goals, all within the requested budget. |

### Tech Writer Recruitment

*How did you find and hire your technical writer? Did the process work well? Did they stay for the duration of the project?*

The hiring of a technical writer presented some challenges to us.

- One pain point were the legal complexities within Swiss law for hiring people outside our country and the EU, which was challenging since a significant portion of interested writers were, e.g., from India.  
- Another pain point was the very high number of requests making it difficult to devote enough time to evaluate each application.   
- A last worrying point was that several applications seemed to be clearly uninspired output of LLM tools, with accompanying letters sounding like chatbot reformulations of our proposal. In the context of the process of hiring a writer, we would have preferred seeing a demonstration of their text-writing skills, rather than their ability to write AI prompts.

Luckily for us, through a local network of teachers and trainers we managed to connect with a technical writer, namely van Geest consultancy, who has experience in designing courses in the field of bioinformatics. We have seen examples of his output in the past, and we knew that he would be a good match for this project.  
This technical writer stayed until the completion of this writing project, including the additional goals.

### Other Participants

*Who else worked on this project (use usernames if requested by participants)? How did you recruit them? What roles did they have? Did they stay for the duration of the project?* 

PD Dr. Katja Baerenfaller leads the Molecular Allergology group at the Swiss Institute of Allergy and Asthma Research (SIAF) in Davos, which is affiliated with the University of Zurich. She teaches the module CDS303 *Data Science und Informatik in der Biology* at the University of Applied Sciences of the Grisons. In the fall semester of 2023, she assigned students the task of analyzing wastewater sequencing data. This data had been acquired in summer 2022 as part of the Grisons wastewater monitoring efforts, in which she was actively involved. For this task, the students were required to use V-pipe, which proved to be quite challenging. Their feedback helped shape the goals for our documentation, including the tasks we incorporated into our proposal.   
For the assignment in the fall semester of 2024, handed out in October with a due date for submitting their reports by the end of November, the new cohort of students had access to the new tutorials and documentation developed as part of this proposal. This allows us to evaluate their effectiveness for users who are inexperienced with our pipeline.

### Timeline

*Give a short overview of the timeline of your project (indicate estimated end date or intermediate milestones if project is ongoing). Did the original timeline need adjustment?*

Due to initial difficulties until we successfully hired a suitable technical writer, we needed to postpone the steps on our timeline (see the updated timeline on the proposal URL).

Onboarding of the writer was postponed to July and start of writing itself was postponed to August.  
As the writer was able to take on the additional goals, including integration to our CI/CD process (running the new tutorial automatically as end-to-end tests), the final deliverable will be available in December.

Unrelated changes on our side, such as expanding the national program of wastewater-based surveillance of viral variants to include respiratory viruses RSV and Influenza and the hiring and onboarding of a new developer will delay the final merging and publication of the deliverable to December.

Despite the shifts in the timeline, we remain happy with the results of this project.

### Deliverables

#### Planned Deliverables

*Relevant links might include published docs, pull requests, or other artifacts.*

| Deliverable | % Complete | Relevant Links  | Notes |
| :---- | :---- | :---- | :---- |
| Branch with new documentation | 100% | [https://github.com/GeertvanGeest/V-pipe/tree/gsod-rtd](https://github.com/GeertvanGeest/V-pipe/tree/gsod-rtd) | Main tasks of the proposal and additional goals are complete by the writer. The integration of the additional goals are being finalized on our side. |
| Read-the-docs deployment | 100% | [https://gsod-vpipe.readthedocs.io/](https://gsod-vpipe.readthedocs.io/) | Completed, will be transferred to V-pipe.readthedocs.io and linked from https://cbg-ethz.github.io/V-pipe/ |
| Automatic integration of config manual | 100% | [https://github.com/GeertvanGeest/V-pipe/actions/runs/11650277793/job/32438805759](https://github.com/GeertvanGeest/V-pipe/actions/runs/11650277793/job/32438805759) | This link is a demonstration of the GitHub workflow running |

#### Unplanned Deliverables

*Were there any deliverables created that were not planned at the start of the project? If so, please explain.* 

To simplify running on a laptop the writer also prepared a download package with data to be used as part of the tutorial, available on an Amazon S3: [https://vpipe-gsod.s3.eu-central-1.amazonaws.com/cowwid\_tutorial.tar.gz](https://vpipe-gsod.s3.eu-central-1.amazonaws.com/cowwid_tutorial.tar.gz)

### Metrics

*What metrics did you choose to measure the success of the project? Were you able to collect those metrics? Did you observe any change as a result of the project? Did you add or remove any metrics since your proposal? How often do you intend to collect metrics going forward?*

The use of V-pipe in the assignment that Prof. Baerenfeller gives to her students at the University of Applied Sciences of Grison gave us a good opportunity to evaluate the documentation.

In 2023, the students used the old documentation during the assignment. They opened 2 issues on V-pipe’s GitHub tracker, and they mentioned difficulties in generating the definition of variants as something that would need improvement.

In 2024, the students used the new documentation written as part of this project. No issue opened by students on the GitHub tracker over the duration of the assignment. In 2024, only two out of 15 students reported being unable to run V-pipe, primarily due to the use of an Apple Silicon Mac, which is a hardware limitation beyond the scope of the documentation of the current GSoD proposal and will be handled instead in a future release of V-pipe. This represents a considerable improvement compared to 2023, when even the students who managed to run V-pipe reported encountering considerable difficulties.  

These before/after snapshots give us a positive evaluation of the deliverables.

In addition, we are taking part in a pair of reproducibility hackathons.  
During the Swiss bioinformatics summit 2024 in June, we tasked participants (a small group of researchers in the field of bioinformatics) to reproduce wastewater analysis. They were provided with the old documentation.  
The next round will take place in February 2025 and the participants (different small groups of similar compositions) will be provided with the new documentations.

An observable impact of the new documentation was during the Elixir BioHackathon Europe 2024 were we worked on integrating V-pipe in cloud-based processing. An online participant offered to help setup submitting the V-pipe’s docker container on a Task Execution Service (TES). After overcoming an initial setback with the download package of the tutorial being down, she managed to follow the tutorials. She successfully learned to use V-pipe’s container and set up the TES submission on her own without needing additional help.

We plan to continue evaluating the impact of the new documentation as third party labs replicate our research. This includes both current partner labs, such as those in Davos , and any upcoming external laboratories. The aim is to onboard new users without needing to book a video-conference call with the developers of V-pipe.

# Analysis

*Provide a short narrative about how the project went. Was the project successful? Why or why not? Or when will you be able to judge success? Did you face any unexpected hurdles or setbacks? Did the project result in any new or updated processes or procedures in your organization?*

Overall we are very happy with the outcome of the current project.

The new documentation on Read the Docs looks much more professional, and is already simplifying the onboarding of new users, as demonstrated in the metrics section above.

The hiring process was tiresome, but once we leveragedour network of connections among teachers and trainers, the rest of the process was smooth thanks to the experienced writer, and regular communications over both chat (Slack) and video calls (Microsoft Teams).

Unrelated difficulties on our side caused delays in integrating and publishing the deliverables that the writer provided us, but aside from the timeline shift, the project was a success.

In the future, we expect that we will be able to point new users to this documentation instead of needing to organise video calls with the developers.

### Lessons Learned


#### What went well?

| Topic | What we did | Lesson Learned |
| :---- | :---- | :---- |
| Budget | Plan for a small and very well-defined tasks | Planning as a small and well-defined main task allowed us to fit well within budget while staying at the lower end of GSoD range of grants. |
| Communication | Regular chat and video calls | Keeping regular contact helped us keep in sync and incorporate feedback |
| Mentorship |  |  |
| Metrics | Plan before/after snapshots | The use of our pipeline by a lecturer as part of a student’s course assignment gave a good opportunity to evaluate old and new documentation |
| Onboarding | Plan enough time for the peculiarities | We managed to get the writer familiarized with some unusual aspects: tutorials are automatically run as CI/CD, and configuration manual is auto-generated |
| Participants | We contacted a teacher who is using our workflow in her course’s assignments | This provided us a very good evaluation opportunity (see Metrics) |
| Project Deliverables | Very clear set of goals from the onset of the project. | Clear goals and deliverables increased our change of success |
| Project Management | Agile approach, no micromanagement | As the writer is experienced, regular communication was enough |
| Recruiting & Hiring | Leveraged our network of contacts | Getting in touch with a writer with known experience and whose trainings quality we know was successful |
| … |  |  |
| Other |  |  |
|  |  |  |
|  |  |  |


#### What could be improved?

| Topic | What we did | What we would do differently | Lesson Learned |
| :---- | :---- | :---- | :---- |
| Budget |  |  |  |
| Communication |  |  |  |
| Mentorship |  |  |  |
| Metrics |  | Planned to do a survey of users | Setting up a whole survey of users with assigned tasks is time and resources consuming. Leveraging reproducibility hackathon was a good fall back giving similar results. |
| Onboarding |  |  |  |
| Participants |  |  |  |
| Project Deliverables |  |  |  |
| Project Management |  |  |  |
| Recruiting & Hiring | As suggested we announced our project publicly and let interested writers contact us. | Probably discuss the submission in advance with a potential writer from our network of teachers and trainers, instead of counting on a fully open recruitment process. | This leads to a very large amount of submissions. Some of them coming from region causing difficulties in hiring process in regard to Swiss law. Some of them of very low qualities (potential writers submitting LLM slop) |
| … |  |  |  |
| Other |  |  |  |
|  |  |  |  |
|  |  |  |  |


