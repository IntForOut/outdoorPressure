## A Knowledge Graph to support the study of human recreational activities in the French Alps and their impact

This Knowledge Graph (KG), see outdoorPressure.rdf, supports the discovery and reuse of data, tools and related expertise to study the impact of recreational activities in the french Alps. 

![Overview of the OutdoorPressure KG main concepts](docs/img/schema_modele_kg.png)

### Want to explore the Knowledge Graph?

Classical ontology documentation : [OutdoorPressure ontology](https://intforout.github.io/outdoorPressure/index.html). 
Dedicated companion software to explore catalogued assets through predefined queries : [here](https://github.com/intForOut/sham-wah).  

### Contribute  

Anyone can contribute by creating issues on this git that will be moderated by the KG curators.
If you wish to contribute specifically with new instances:
- create one or more **UserFeedback** instances for sharing your expertise, experience, or observations about data or about papers you read. Follow the steps described [here](./docs/new_userfeedback.md)
- create one or more **Dataset** to describe data that is relevant to the scope. A dataset is "a coherent collection of information or resources (data files, explanatory files, APIs, links, etc.) and metadata (description, publication date, keywords, geographical/temporal coverage, etc.)." Follow the steps described  [here](./docs/new_dataset.md)  
  
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
