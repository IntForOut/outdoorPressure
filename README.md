# A Knowledge Graph to support the study of human recreational activities in the French Alps and their impact

This is research Knowledge Graph (KG) to support the study of human outdoor leisure in the French Alps and its impact. It aims at supporting the discovery and proper reuse of data, ranging from GPS collar to camera trap and land cover data. It embeds concepts relevant to express users interests in real world phenomena, like "human activities". It also catalogues different assets relevant to their study like datasets, reproducible processes, scientific papers, or the experience and feedback from other users.

![Overview of the OutdoorPressure KG main concepts](docs/img/ODKG-schemaGeneral-horizontal.png)

### Want to explore the Knowledge Graph?

The KG is in the rdf file outdoorPressure.rdf in this github repository. There is a documentation attached to it [OutdoorPressure ontology](https://intforout.github.io/outdoorPressure/index.html). 

We recommand you use/test a companion software to explore it [here](https://github.com/intForOut/sham-wah). Sham-Wah is a work in progress to ease the way people who are not Knowledge Graph experts can query and explore visually the KG. 

### Contribute with concepts 

The philosophy of the KG is to be open. Currently, Intforout participants can contribute to the edition/revision of concepts (classes, object properties, data properties) during webinars organized by the KG moderators, or by creating issues on this git. 

### Contribute with instances 

The easiest way to contribute is with new instances:
- create one or more **UserFeedback** instances for sharing your expertise, experience, or observations about data or about papers you read. Follow the steps described [here](./docs/new_userfeedback.md)
- create one or more **Dataset** to describe data that is relevant to the scope. A dataset is "a coherent collection of information or resources (data files, explanatory files, APIs, links, etc.) and metadata (description, publication date, keywords, geographical/temporal coverage, etc.)." Follow the steps described  [here](./docs/new_dataset.md)  
  
### Report issues or propose improvements

If you have encounters bugs or problemes in the KG such as:

- a node with incorrect properties (e.g: wrong description, wrong type such as dataservice instead of dataset)
- incorrect or missing links
- data that should represents another concept (e.g: representing animal activity instead of human activity)
- or if you want to propose a new concept

Please open a GitHub issue (using either the bug-report issue template or a blank issue) so the moderators can review and take the appropriate action.
​
Open the Github Issue tab as shown below:

<p align='left' style="margin-top: 20px;">
<img src="docs/img/issue_github.png" alt="issue github" width="500">
</p>

### Acknowledgements

This work was supported by the ANR research project **[IntForOut](https://www.umr-lastig.fr/intforout/)**: Multisource spatial data INTegration FOR the Monitoring of Ecosystems under the pressure of OUTdoor recreation (ANR-23-CE55-0003).
