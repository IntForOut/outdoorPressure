# Propose to describe a new dataset in the KG

It is up to you to decide what is your dataset. We recommand you do not create too many datasets. When you have several files that altogether are a relevant coherent set to be used together, this is very good candidate for a dataset. There can be different files with different schemas in it. The description can further explain this and how data is organised in different files. See definition of a dataset from the french research data portal : "a coherent collection of information or resources (data files, explanatory files, APIs, links, etc.) and metadata (description, publication date, keywords, geographical/temporal coverage, etc.)." See DCAT definition : "A collection of data, published or curated by a single agent, and available for access or download in one or more representations."   

Other resources can be useful to describe data : a dataseries is a collection of datasets that share similar characteristics, like maps on different places (see https://www.w3.org/TR/vocab-dcat-3/#dataset-series) or the relationship version between datasets. 

Collect the description items listed in the section below and send it to us using the form template available through the GitHub “Issue” button. We will use this information to update the Knowledge Graph. To access the form, open the Issues tab as shown below:

<p align='left' style="margin-top: 20px;">
<img src="../docs/img/issue_github.png" alt="Architecture Diagram of Sham-Wah" width="500">
</p>

# Description items we need to create the KG instances 

1. **URI**: please suggest a short name that makes sense for human beyond a too specific context, so avoid "CarlsData" or "myowndata", whenever it is possible use words that indicate : theme, place, years. 

2. **Label**: short name for your dataset

3. **Comment**: description of your dataset, you can also express here if it comes with specific metadata or documentation.

4. **Distribution**: tell if it is on the ftp with a specific file name (or folder), if it is available through a download service or dataservice, if it comes with specific documentation and structured metadata. Note that we won't necessary load as KG nodes and edges these metadata, they can remain in their native format.

5. **Location** : Spatial extent of the dataset

6. **Author**: Check whether the corresponding Person node already exists in the Knowledge Graph. If not, propose an IRI and we will add it.

7. **Issue/Date** : date of last update of the dataset

8. **Represents** : please express if your dataset represents Land entities, animal or human activities 

