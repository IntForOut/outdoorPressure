# Tutorials

- [Create a new instance of dataset](NewDataset)
- [Create a new instance of userfeedback](NewUserFeedback)

## CreateIssue 
For any new instance, you can prepare required description items listed in the section below and send it using the form template available through the GitHub “Issue” button. To access the form, open the Issues tab as shown below:
<p align='left' style="margin-top: 20px;">
<img src="../docs/img/issue_github.png" alt="Architecture Diagram of Sham-Wah" width="500">
</p>

##  NewDataset

It is up to you to decide what is your *Dataset*. We recommand you do not create too many datasets. When you have several files that altogether are a relevant coherent set to be used together, this is very good candidate for a dataset. There can be different files with different schemas in it. The description can further explain this and how data is organised in different files. See definition of a dataset from the french research data portal : "a coherent collection of information or resources (data files, explanatory files, APIs, links, etc.) and metadata (description, publication date, keywords, geographical/temporal coverage, etc.)." See DCAT definition : "A collection of data, published or curated by a single agent, and available for access or download in one or more representations."  You can also want to create a *Dataseries* is a collection of datasets that share similar characteristics, like maps on different places (see https://www.w3.org/TR/vocab-dcat-3/#dataset-series) or the relationship version between datasets. 
1. **URI**: please suggest a short name that makes sense for human beyond a too specific context, so avoid "CarlsData" or "myowndata", whenever it is possible use words that combine : product or provider (like BDTopo, Strava, etc), theme (like HumanIbexEncounter, Tracks, etc), place, years. In the case where a dataset is well identified by a published work it is possible also to use it as identifier for example "DataPhdKerouanton".
2. **Label**: short name for your dataset
3. **Comment**: description of your dataset, if it is organised in different parts, that may correspond to different files in its distribution. You can also express here if it comes with specific metadata or documentation. 
4. **Distribution**: tell if it is on the ftp with a specific file name (or folder), if it is available through a download service or dataservice
5. **Location** : Spatial extent of the dataset
6. **Author**: Check whether the corresponding Person node already exists in the Knowledge Graph. If not, propose an IRI and we will add it.
7. **Issue/Date** : date of last update of the dataset
8. **Represents** : please express if your dataset represents Land entities, animal or human activities 

## NewUserFeedback

If you want to share your expertise, experience, or observations about data, you can do so by proposing a User Feedback within the Knowledge Graph. This concept is based on the [Geospatial User Feedback (GUF)](https://www.ogc.org/standards/guf/) model which emphasizes clear human-readable comments, explicit links to the data being discussed. You can include comments on data quality (completeness or accuracy), suggestions for improving data processing, observations about how datasets can be combined or reused and remarks on reproducibility or potential applications. It builds community intelligence.
1. **URI**: please suggest a short informative name. e.g. **https://intforout.github.io/outdoorPressure#ProfilageDonneesKerouantonANaciri**
2. **Comment**: A clear description of your observation, including which data or process you are referring to.
3. **Author**: Check whether the corresponding Person node already exists in the Knowledge Graph. If not, propose an IRI.
4. **Targets**: The elements your feedback refers to, such as one or more data (datasets, services, processes, etc.) mentioned in your feedback and/or a file (eg. PDF file report) you are commenting on

If a target is a document, you can upload it to the issue or directly into technical-documents in this github.
If a target is data that is not yet referenced in the Knowledge Graph, please provide the necessary information to create the corresponding node. 
If your User Feedback is about data that already exists in the Knowledge Graph, you can locate the corresponding IRI in several ways :  1)Consult the Knowledge Graph [raw file](https://intforout.github.io/outdoorPressure/outdoorPressure.rdf), 2) read the [documentation](https://intforout.github.io/outdoorPressure/index.html) 3) Explore the Knowledge Graph Companion [Sham‑Wah](https://github.com/IntForOut/sham-wah) *Note: Sham‑Wah is still under active development. It currently focuses on predefined queries, mainly related to human‑activity data. Because both Sham‑Wah and the Knowledge Graph are evolving, not all data nodes or concepts are fully linked or visible yet. As a result, you may not find every data in the interface for now.*


