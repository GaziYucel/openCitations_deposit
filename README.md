# Open Citations Croci Depot

This example is created to show an alternate way of transmitting citations to Open Citations CROCI from within Open Journal Systems (OJS) through the plugin OptimetaCitations. As this is an proposal, all data formats below are open for discussion. Please also see the example issues. 

**title**

After an article is issued a DOI and published in OJS, the citations are published to this Github reporistory as an issue. The title will be in the following format: "deposit {domain name of journal} {doi or other identifier}". For example "deposit localhost:330 doi:10.1007/978-3-030-00668-6_8"

**body**

The body will consist of the metadata of the article and the citations in JSON form. 
The structure is an combination of META-CSV and CITS-CSV as described https://arxiv.org/abs/2206.03971.

```
[ 
  {
    "ids": { "doi": "10.1007/978-3-030-00668-6_8" },
    "title": "The SPAR Ontologies",
    "author": [ 
      { "name": "Peroni, Silvio", "ids": { "orcid": "0000-0003-0530-4305" } } , 
      { "name": "Shotton, David", "ids": { "orcid":"0000-0001-5506-523X" } } ],
    "pub_date": "2018",
    "venue": [ 
      { "name": "17th ISWC", "ids": { "doi": "10.1007/978-3-030-00668-6" } } ],
    "volume": "1",
    "issue": "1-2",
    "page": "119-136",
    "type": "book chapter",
    "publisher": [ 
      { "name": "Springer International Publishing", "ids": { "crossref": "297" }} ],
    "editor": [ 
      { "name": "Peroni, Silvio", "ids": { "orcid": "0000-0003-0530-4305" } } ],
    "citing": [ 
      { "ids": { "doi": "10.1087/2009202;2009-04-01" }, "date": "2009-04-01", "raw": "" },
      { "ids": { "doi": "10.1371/journal.pcbi.1000361" }, "date": "", "raw": "" },
      { "ids": { "doi": "10.1007/978-3-642-33876-2_35" }, "date": "2012", "raw": "" },
      { "ids": { "doi": "10.1186/2041-1480-1-S1-S6" }, "date": "2010-06-22", "raw": "" },
      { "ids": { "doi": "10.1145/945645.945664" }, "date": "2003-10-23", "raw": "" },
      { "ids": {}, "date": "", "raw": "Gangemi, A., Peroni, S., Vitali, F.: Literal reification. In: Proceedings of WOP 2010, pp. 65–66 (2010). http://ceur-ws.org/Vol-671/pat04.pdf" },
      { "ids": {}, "date": "", "raw": "Hammond, T., Pasin, M.: The nature.com ontologies portal. In: Proceedings of LISC 2015 (2015). http://ceur-ws.org/Vol-1572/paper2.pdf" } ]
  } 
]
```
**label**

The label 'Deposit' will be added to the issue. 

**next steps**
Open Citations will then download and process this data and after processing mark the issue 'Done'. The deposit could also be rejected by marking the message 'Rejected'.

**history**

A history of all the deposits could be kept by doing the following. After processing an deposit, an entry in the Wiki could be made with a link to OpenCitations CROCI API with the DOI or other Identifier. The original issue can be removed after this. 
