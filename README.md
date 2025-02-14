# Open Citations Croci Depot

This example is created to show an alternate way of transmitting citations to Open Citations CROCI from within Open Journal Systems (OJS) through the plugin OptimetaCitations. As this is an proposal, all data formats below are open for discussion. Please also see the example issues. 

This issue will be an example which we will be using: https://github.com/GaziYucel/open_citations_croci_depot/issues/15

**issue:title**

After an article is issued a DOI and published in OJS, the citations are published to this Github reporistory as an issue. The title will be in the following format: "deposit {domain name of journal} {doi or other identifier}". For example "deposit localhost:330 doi:10.1007/978-3-030-00668-6_8"

**issue:body**

The body will consist of the metadata of the article and the citations in CSV. The two will be separated by an unique separator. See example below.


```
"id","title","author","pub_date","venue","volume","issue","page","type","publisher","editor"
"doi:10.1007/978-3-662-07918-8_3","Influence of Dielectric Properties, State, and Electrodes on Electric Strength","Ushakov, Vasily Y.","2004","Insulation of High-Voltage Equipment [isbn:9783642058530 isbn:9783662079188]","","","27-82","book chapter","Springer Science and Business Media LLC [crossref:297]",""
"doi:10.1016/0021-9991(73)90147-2","Flux-corrected transport. I. SHASTA, a fluid transport algorithm that works","Boris, Jay P; Book, David L","1973-1","Journal of Computational Physics [issn:0021-9991]","11","1","38-69","journal article","Elsevier BV [crossref:78]",""
"doi:10.1109/20.877674","An investigation of FEM-FCT method for streamer corona simulation","Woong-Gee Min, ; Hyeong-Seok Kim, ; Seok-Hyun Lee, ; Song-Yop Hahn, ","2000-7","IEEE Transactions on Magnetics [issn:0018-9464]","36","4","1280-1284","journal article","Institute of Electrical and Electronics Engineers (IEEE) [crossref:263]",""
"doi:10.1109/tps.2003.815469","Numerical study on influences of barrier arrangements on dielectric barrier discharge characteristics","Woo Seok Kang, ; Jin Myung Park, ; Yongho Kim, ; Sang Hee Hong, ","2003-8","IEEE Transactions on Plasma Science [issn:0093-3813]","31","4","504-510","journal article","Institute of Electrical and Electronics Engineers (IEEE) [crossref:263]",""
"","Spatial Distribution of Ion Current Around HVDC Bundle Conductors","Zhou, Xiangxian; Cui, Xiang; Lu, Tiebing; Fang, Chao; Zhen, Yongzan","2012-1","IEEE Transactions on Power Delivery [issn:0885-8977 issn:1937-4208]","27","1","380-390","journal article","Institute of Electrical and Electronics Engineers (IEEE) [crossref:263]",""
"doi:10.1007/978-1-4615-3786-1_11","The Solution of the Continuity Equations in Ionization and Plasma Growth","Davies, A. J.; Niessen, W.","1990","Physics and Applications of Pseudosparks [isbn:9781461366874 isbn:9781461537861]","","","197-217","book chapter","Springer Science and Business Media LLC [crossref:297]",""
"doi:10.1088/0022-3727/13/1/002","Discharge current induced by the motion of charged particles","Sato, N","1980-1-14","Journal of Physics D: Applied Physics [issn:0022-3727 issn:1361-6463]","13","1","3-6","journal article","IOP Publishing [crossref:266]",""
"doi:10.1109/27.106800","Particle-in-cell charged-particle simulations, plus Monte Carlo collisions with neutral atoms, PIC-MCC","Birdsall, C.K.","1991-4","IEEE Transactions on Plasma Science [issn:0093-3813]","19","2","65-85","journal article","Institute of Electrical and Electronics Engineers (IEEE) [crossref:263]",""
"doi:10.1016/0021-9991(79)90051-2","Fully multidimensional flux-corrected transport algorithms for fluids","Zalesak, Steven T","1979-6","Journal of Computational Physics [issn:0021-9991]","31","3","335-362","journal article","Elsevier BV [crossref:78]",""
"doi:10.1088/0022-3727/39/14/017","Diffusion correction to the Raether–Meek criterion for the avalanche-to-streamer transition","Montijn, Carolynne; Ebert, Ute [orcid:0000-0003-3891-6869]","2006-6-30","Journal of Physics D: Applied Physics [issn:0022-3727 issn:1361-6463]","39","14","2979-2992","journal article","IOP Publishing [crossref:266]",""
"doi:10.1007/978-3-663-14090-0 isbn:9783528085995 isbn:9783663140900","High-Voltage Insulation Technology","Kind, Dieter; Kärner, Hermann","1985","","","","","book","Springer Science and Business Media LLC [crossref:297]",""
"","Space-charge effects in high-density plasmas","Morrow, R","1982-6","Journal of Computational Physics [issn:0021-9991]","46","3","454-461","journal article","Elsevier BV [crossref:78]",""
"doi:10.1007/s42835-022-01029-y","Numerical Simulation of Gas Discharge Using SUPG-FEM-FCT Method with Adaptive Mesh Refinement","Choi, Chan Young; Park, Il Han [orcid:0000-0002-9383-6856]","2022-2-28","Journal of Electrical Engineering & Technology [issn:1975-0102 issn:2093-7423]","17","3","1873-1881","journal article","Springer Science and Business Media LLC [crossref:297]",""
===###===@@@===
"citing_id","citing_publication_date","cited_id","cited_publication_date"
"doi:10.1007/s42835-022-01029-y","2022-02-28","doi:10.1007/978-3-662-07918-8_3","2004"
"doi:10.1007/s42835-022-01029-y","2022-02-28","doi:10.1016/0021-9991(73)90147-2","1973-1"
"doi:10.1007/s42835-022-01029-y","2022-02-28","doi:10.1109/20.877674","2000-7"
"doi:10.1007/s42835-022-01029-y","2022-02-28","doi:10.1109/tps.2003.815469",""
"doi:10.1007/s42835-022-01029-y","2022-02-28","doi:10.1109/tpwrd.2011.2172694","2012-1"
"doi:10.1007/s42835-022-01029-y","2022-02-28","doi:10.1007/978-1-4615-3786-1_11","1990"
"doi:10.1007/s42835-022-01029-y","2022-02-28","doi:10.1088/0022-3727/13/1/002","1980-1-14"
"doi:10.1007/s42835-022-01029-y","2022-02-28","doi:10.1109/27.106800","1991-4"
"doi:10.1007/s42835-022-01029-y","2022-02-28","doi:10.1016/0021-9991(79)90051-2","1979-6"
"doi:10.1007/s42835-022-01029-y","2022-02-28","doi:10.1088/0022-3727/39/14/017",""
"doi:10.1007/s42835-022-01029-y","2022-02-28","doi:10.1007/978-3-663-14090-0","1985"
"doi:10.1007/s42835-022-01029-y","2022-02-28","doi:10.1016/0021-9991(82)90026-2",""
```
**issue:label**

The label 'Deposit' will be added to the issue. 

**next steps**

Open Citations will then download and process this data and after processing mark the issue 'Done'. The deposit could also be rejected by marking the message 'Rejected'.

**history**

A history of all the deposits could be kept by doing the following. After processing an deposit, an entry in the Wiki could be made with a link to OpenCitations CROCI API with the DOI or other Identifier. The original issue can be removed after this. With this process, the size of this repository can be kept small and keep the history. 
