
# IoT-F: IoT Failure Ontology ontology
The IoT failure Management ontology (IoT-F) aims to provide a reference model for the IoT failure management domain. Device manufacturers will use this shared model to build a shared knowledge base, enabling efficient IoT failure diagnosis and IoT failure impact analysis. More precisely, it enables the following usages:
 1. Connect distributed and heterogeneous IoT failure diagnosis information governed by different device manufacturers.
 2. Help IoT device manufacturers in structuring IoT device failure information.
 3. Enable efficient search for recovery plans, failure cause, and its impact given a failed device type and a set of monitoring indicators thanks to the knowledge graph structure.  
 4. Allow our cooperative agents [OSAMA](https://github.com/Orange-OpenSource/collaborativeDM-OSAMA-agent) to understand failure data to perform collaborative and automatic cascading failure recovery.
![alt text](https://github.com/Orange-OpenSource/collaborativeDM-IoTF-ontology-documentation/blob/master/iotf.png?raw=true)
The ontology documentation is built using the [Widoco](https://github.com/dgarijo/Widoco) toolset, and can be accessed via [IoT-F Ontology](https://iotfontology.github.io/).
# Diagnosis Sparql Query
```
"PREFIX rdf: <http://www.w3.org/1999/02/22-rdf-syntax-ns#>"+
                             "PREFIX owl: <http://www.w3.org/2002/07/owl#>"+
                             "PREFIX rdfs: <http://www.w3.org/2000/01/rdf-schema#>"+
                             "PREFIX xsd: <http://www.w3.org/2001/XMLSchema#>"+
                             "PREFIX iotf: <http://www.semanticweb.org/orangeinnovation/IoTF#>\n"+
"SELECT ?deviceType ?failureMode ?recoveryAction [Failure Symptoms ex: ?failureCode]"+
  "WHERE { ?failureMode rdf:type iotf:FailureMode."+
      "?failureMode iotf:hasRecoveryAction ?recoveryAction."+
      "?failureMode iotf:happensAt ?deviceType."+
      "OPTIONAL {?failureMode iotf:hasFailureSymptom [Failure Symptoms ex: ?failureCode]. }"+
      "Filter([a set of failure sympthoms])}";
```
## License
 
 This software is distributed under [BSD-3-Clause](LICENCE). 

Copyright (c) 2023 Orange


## Maintainer
 
 * Amal GUITTOUM e-mail: amal.guittoum@orange.com
