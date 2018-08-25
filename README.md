# Australian Government Epochs Dataset
This is a Linked Data dataset that contains representations of epochs relevant to Australian government, such as the political markers of Prime Ministerships and pop-culture time periods like the Cold War.

*As of August, 2018, this dataset is at a very early stage of development and while this abstract is written as if the dataset is complete and functioning, it is not.*

This dataset is composed of multiple, named, *timescales* split into *epochs* with relations between them represented using <a href="https://doi.org/10.1016/0004-3702(84)90008-0">Allen's interval algebra</a>. The dataset uses the [Resource Description Framework (RDF)](https://www.w3.org/RDF/) for all data and makes use of the [Time Ontology in OWL](https://www.w3.org/TR/owl-time/) and well known upper ontologies for its modelling.

Each *timescales* and *epoch* is identified using a persistent URI (PID URI) which is a long-term stable web address issued by the [Australian Government Linked Data Working Group](http://www.linked.data.gov.au). This means that even when technologies and organisations change, the timescales and epochs will be able to be referred to and linked to via web addresses such as this for the Prime Ministerships timescale:

```
http://linked.data.gov.au/dataset/epochs/trs/prime-ministerships
```

The dataset delivers the Prime Ministerships timescale as a Temporal Reference System (hence the URI path segment 'trs') and the URI above delivers information about that timescale/trs. For all the individual Prime Ministerships within that timescale, a slash '/', is appended to the timescale URI to indicate that a register of all its constituent parts, in this case Prime Ministerships, is requested.


The dataset itself is identified by the PID URI that is the base for all timescales and epoch PID URIs, namely:

```
http://linked.data.gov.au/dataset/epochs
```

From there, the landing page of the dataset, you can find links to all of its content.


## Motivation and expected use
This dataset has been developed to act as a temporal reference system for several Australian government Linked Data projects. Those projects need to be able to extract time slices of datasets such as the *Australian Government Organisations Register in OWL* (not built yet) using queries of the form:

```
get me the Australian Federal Government Departments,
as they were during the Keating Prime Ministership
```

Here an imagined dataset containing Australian Federal Government Departments (*Departments* being the Australian equivalent of other government's *Ministries*) is queries for the list of those Departments, as they were during the *Keating Prime Ministership*, the time period in which Paul Keating was Prime Minister (1991 - 1996). Since this time period, or *epoch* was length, 5 years, and Departments changed during that time, one could expect such a query to return multiple lists of Departments, one for every configuration during that epoch.

Since this dataset related all its *epochs* in all *timescales* to two numerical timescales - the [Gregorian Calendar](https://en.wikipedia.org/wiki/Gregorian_calendar) and [Unix time](https://en.wikipedia.org/wiki/Unix_time) - calculations across any timescales and queries with numerical dates are possible.


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
