# Australian Government Epochs Dataset
This is a Linked Data dataset that contains representations of epochs relevant to Australian government, such as the political markers of Prime Ministerships and pop-culture time periods like the Cold War.

*As of August, 2018, this dataset is at a very early stage of development and while this abstract is written as if the dataset is complete and functioning, it is not.*

This dataset is composed of multiple, named, *timelines* split into *epochs* with relations between them represented using <a href="https://doi.org/10.1016/0004-3702(84)90008-0">Allen's interval algebra</a>. The dataset uses the [Resource Description Framework (RDF)](https://www.w3.org/RDF/) for all data and makes use of the [Time Ontology in OWL](https://www.w3.org/TR/owl-time/) and well known upper ontologies for its modelling.

Each *timeline* and *epoch* is identified using a persistent URI (PID URI) which is a long-term stable web address issued by the [Australian Government Linked Data Working Group](http://www.linked.data.gov.au). This means that even when technologies and organisations change, the timelines and epochs will be able to be referred to and linked to via web addresses such as this for the Prime Ministerial timeline:

```
http://linked.data.gov.au/dataset/epochs/prime-ministerships
```

The dataset itself is identified by the PID URI that is the base for all timeline and epoch PID URIs, namely:

```
http://linked.data.gov.au/dataset/epochs
```

From there, the landing page of the dataset, you can find links to all of its content.


## Motivation and expected use
This dataset has been developed to act as a temporal reference system for several Australian government Linked Data projects. Those projects need to be able to extract time slices of datasets such as the *Australian Government Organisations Register in OWL* (not built yet) using queries of the form:

```
get me the Australian Federal Government Departments,
as they were during the Keating government
```

Such queries use well-known epochs to describe time periods, rather than numerical time values. This dataset provides fixity for those epochs and relates them to numerical time.


## License
The content of this API is licensed for use under the [Creative Commons 4.0 License](https://creativecommons.org/licenses/by/4.0/). See the [license deed](LICENSE) all details.


## Citation
If you wish to cite this ontology, please do so like this:

Car, N.J. & Cox, S.J.D. (2018) "Australian Government Epochs Dataset". An RDF datasets using the Web Ontology Language. http://linked.data.gov.au/dataset/epochs


## Contacts
**Nicholas Car**  
CSIRO Land & Water  
*author*  
<nicholas.car@csiro.au>

**Simon Cox**  
CSIRO Land & Water  
*author*  
<simon.cox@csiro.au>
