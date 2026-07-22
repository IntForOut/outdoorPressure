# Tutorials

- [Create a new instance of dataset](new_dataset.md)
- [Create a new instance of userfeedback](new_userfeedback.md)


#  Create a new instance of dataset

It is up to you to decide what is your dataset. We recommand you do not create too many datasets. When you have several files that altogether are a relevant coherent set to be used together, this is very good candidate for a dataset. There can be different files with different schemas in it. The description can further explain this and how data is organised in different files. See definition of a dataset from the french research data portal : "a coherent collection of information or resources (data files, explanatory files, APIs, links, etc.) and metadata (description, publication date, keywords, geographical/temporal coverage, etc.)." See DCAT definition : "A collection of data, published or curated by a single agent, and available for access or download in one or more representations."   

Other resources can be useful to describe data : a dataseries is a collection of datasets that share similar characteristics, like maps on different places (see https://www.w3.org/TR/vocab-dcat-3/#dataset-series) or the relationship version between datasets. 

Collect the description items listed in the section below and send it to us using the form template available through the GitHub “Issue” button. We will use this information to update the Knowledge Graph. To access the form, open the Issues tab as shown below:

<p align='left' style="margin-top: 20px;">
<img src="../docs/img/issue_github.png" alt="Architecture Diagram of Sham-Wah" width="500">
</p>

**Description items for your dataset** 

1. **URI**: please suggest a short name that makes sense for human beyond a too specific context, so avoid "CarlsData" or "myowndata", whenever it is possible use words that combine : product or provider (like BDTopo, Strava, etc), theme (like HumanIbexEncounter, Tracks, etc), place, years. In the case where a dataset is well identified by a published work it is possible also to use it as identifier for example "DataPhdKerouanton".

2. **Label**: short name for your dataset

3. **Comment**: description of your dataset, if it is organised in different parts, that may correspond to different files in its distribution. You can also express here if it comes with specific metadata or documentation. 

4. **Distribution**: tell if it is on the ftp with a specific file name (or folder), if it is available through a download service or dataservice
  
5. **Location** : Spatial extent of the dataset

6. **Author**: Check whether the corresponding Person node already exists in the Knowledge Graph. If not, propose an IRI and we will add it.

7. **Issue/Date** : date of last update of the dataset

8. **Represents** : please express if your dataset represents Land entities, animal or human activities 

# Share Your Expertise Through User Feedback

If you want to share your expertise, experience, or observations about data, you can do so by proposing a User Feedback within the Knowledge Graph. This concept is based on the [Geospatial User Feedback (GUF)](https://www.ogc.org/standards/guf/) model defined by the Open Geospatial Consortium (OGC), which provides a standardized way to capture community knowledge about geospatial resources. It emphasizes clear human-readable comments, explicit links to the data being discussed and interoperability.

Through the UserFeedback, your feedback can include comments on data quality (completeness or accuracy), suggestions for improving data processing, observations about how datasets can be combined or reused and remarks on reproducibility or potential applications. It builds community intelligence which makes the Knowledge Graph richer and valuable.

## How the UserFeedback is represented in the Knowledge Graph ?

To integrate your feedback into the Knowledge Graph, we create a User Feedback node, following the structure inspired by the OGC GUF model. This node includes:

- **Comment**: A clear description of your observation, including which data or process you are referring to.

- **Author**: Your name or identifier, ensuring transparency and traceability.

- **Targets**: The elements your feedback refers to, such as one or more data (datasets, services, processes, etc.) mentioned in your feedback and/or a file (eg. PDF file report) you are commenting on

## How to share your UserFeedback with us ?

Collect the information linked to your UserFeedback and send it to us using the form template available through the GitHub “Issue” button.
We will use this information to update the Knowledge Graph.

To access the form, open the Issues tab as shown below:

<p align='left' style="margin-top: 20px;">
<img src="../docs/img/issue_github.png" alt="Architecture Diagram of Sham-Wah" width="500">
</p>

Then select the appropriate form template:

<p align='left' style="margin-top: 20px;">
<img src="../docs/img/guf_issue.png" alt="Architecture Diagram of Sham-Wah" width="500">
</p>

### Metadata we need to creeate the UserFeedback node

1. IRI for the UserFeedback node (if data-profiling of ressources - Format: “Profilage + DataName + Author”)
   - e.g. **https://intforout.github.io/outdoorPressure#ProfilageDonneesKerouantonANaciri**

2. Comment: A clear description of your observation, including which data or process you are referring to.
   - e.g. **Analyse « profilage » des données de recherche produites par Colin Kerouanton, notamment de la distribution des valeurs (target 1). Le résultat de l’analyse est partagé dans un rapport (target 2).**

3. Author: Check whether the corresponding Person node already exists in the Knowledge Graph. If not, propose an IRI and we will add it.
   - e.g. **https://intforout.github.io/outdoorPressure#anaciri**

4. Targets
   - Target 1 IRI: **https://intforout.github.io/outdoorPressure#KerouantonSurveyFieldCampaignTracksGNSS20142015**
   - Target 2 IRI: **https://intforout.github.io/outdoorPressure#ProfilageDataPhDKerouanton.pdf**
   - There could be more data target if the comment deals with more data

If you have performed data profiling on resources that are represented in the Knowledge Graph and produced a data‑profiling report in PDF format, we will need to create a Document Node to represent your PDF. Therefore, when filling out the issue form, please remember to upload your PDF file, as it is required to create the corresponding node in the Knowledge Graph.

## Where do I found the IRI of the data I'm refering to?

- If the data you are referring to is not already included in the Knowledge Graph, please provide us with the necessary information so we can create the corresponding node. You can do this by sending us a link to the data, the data file itself, its exact name, and its source or origin.

- If your User Feedback is about data that already exists in the Knowledge Graph, you can locate the corresponding IRI in several ways:
  1. Consult the Knowledge Graph documentation [here](https://intforout.github.io/outdoorPressure/index.html)

  2. Explore the Knowledge Graph Companion “Sham‑Wah” [here](https://github.com/IntForOut/sham-wah)

     **Note: Sham‑Wah is still under active development. It currently focuses on predefined queries, mainly related to human‑activity data. Because both Sham‑Wah and the Knowledge Graph are evolving, not all data nodes or concepts are fully linked or visible yet. As a result, you may not find every data in the interface for now.**

  3. Load the RDF file into Protégé

     The RDF file representing the Knowledge Graph is available in this GitHub repository.
     You can download it and open it in Protégé to browse all classes, properties, and individuals, including the IRIs of the data you want to reference.

## Examples of UserFeedbacks

### UserFeedback of Data-Profiling

- IRI: https://intforout.github.io/outdoorPressure#ProfilageDonneesKerouantonANaciri
- Author IRI: https://intforout.github.io/outdoorPressure#anaciri
- Comment:

  "Analyse -profilage- des données de recherche produites par Colin Kerouanton, notamment de la distribution des valeurs, (target 1). Le résultat de l'analyse est partagé dans un rapport (target 2)"

- Target IRI:
  - Target 1: https://intforout.github.io/outdoorPressure#KerouantonSurveyFieldCampaignTracksGNSS20142015
  - Target 2: https://intforout.github.io/outdoorPressure#ProfilageDataPhDKerouanton.pdf

### Quality Of OV Recreational User Map Service

- IRI: https://intforout.github.io/outdoorPressure#QualityOfOVRecreationalUserMapService
- Author: http://purl.org/www.umr-lastig.fr/geodata#mdvandamme
- Comment:

  "Artifacts exist in dense urban areas above a certain zoom level. This is because the accuracy of GPS tracks is lower in these areas, making the spatial information displayed less relevant."

- Target IRI: https://intforout.github.io/outdoorPressure#OVRecreationalUserMapService

### Track Collection Merge For Replicability

- IRI: https://intforout.github.io/outdoorPressure#TrackCollectionMergeForReplicability
- Author: http://purl.org/www.umr-lastig.fr/geodata#mdvandamme
- Comment:

  "The process proposed in this paper can probably be reproduced to generate HikersFootprint in Les Bauges and MontBlanc, using OutdoorVision data as an input"

- Target IRI:
  - Target 1: https://intforout.github.io/outdoorPressure/index.html#OVTracksMontBlancBauges2024
  - Target 2: https://intforout.github.io/outdoorPressure/index.html#SIGSPATIAL24VanDammeEtAl2024

### Ask for clarity about data

- IRI: outdoorPressure#LectureRapportProfilageKerouanton
- Author: https://orcid.org/0000-0002-5797-5170
- Comment:

  "I didn’t understand what the profiling was about"

- Target IRI:
  - Target 1: https://intforout.github.io/outdoorPressure#ProfilageDonneesKerouantonANaciri

### Userfeedback about territorial transformations

- IRI: #ProjetCommunTSI25
- Author IRI: https://orcid.org/0000-0002-5797-5170
- Comment:

  "From local knowledge and aerial photos of the IGN, before (target1), after (target2) description of two transformations in a set of geographical data (target3)
  "

- Target IRI:
  - Target 1: Photographies aériennes historiques 1950-1960 de l'IGN, sur la commune 56730
  - Target 2: Photographies aériennes de l'IGN, sur la commune 56730, consultées le 11/03/26
  - Target 3: TransformationsStGildas.shp

    **Note: If you have created a shapefile to document or illustrate the territorial transformations you observed, you can also share this file with us. This type of user‑generated data is valuable because it supports and enriches your feedback. So, when submitting the issue form, feel free to attach any shapefiles you produced to substantiate your observations.**

