
# IoT-F: IoT Failure Ontology ontology v2 alignment with [saref new version](https://www.etsi.org/deliver/etsi_ts/103200_103299/103264/03.02.01_60/ts_103264v030201p.pdf)
The IoT failure Management ontology (IoT-F) aims to provide a reference model for the IoT failure management domain. Device manufacturers will use this shared model to build a shared knowledge base, enabling efficient IoT failure diagnosis and IoT failure impact analysis. More precisely, it enables the following usages:
 1. Connect distributed and heterogeneous IoT failure diagnosis information governed by different device manufacturers.
 2. Help IoT device manufacturers in structuring IoT device failure information.
 3. Enable efficient search for recovery plans, failure cause, and its impact given a failed device type and a set of monitoring indicators thanks to the knowledge graph structure.  
 4. Allow our cooperative agents [OSAMA](https://github.com/Orange-OpenSource/collaborativeDM-OSAMA-agent) to understand failure data to perform collaborative and automatic cascading failure recovery.
![alt text](https://github.com/Orange-OpenSource/collaborativeDM-IoTF-ontology-documentation/blob/master/iotf.png?raw=true)
The ontology documentation is built using the [Widoco](https://github.com/dgarijo/Widoco) toolset, and can be accessed via [IoT-F Ontology](https://iotfontology.github.io/).
## Main Competency Questions (CQ) of the IoT-F ontology

```
– CQ1. What are managed IoT device type?
– CQ2. For each IoT device type, what are its failure modes?
– CQ3. For each failure modes, what are it associated symptoms?
– CQ4. For each failure mode, what are its effects?
– CQ5. For each failure mode, what are its causes?
– CQ6. For each failure mode, what are its possible recovery actions?
```
## License
 
 This software is distributed under [BSD-3-Clause](LICENCE). 

Copyright (c) 2023 Orange


## Maintainer
 
 * Amal GUITTOUM e-mail: amal.guittoum@orange.com
