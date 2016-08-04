# What is ml-cyber?

Used to demonstrate importing multiple cyber and non-cyber ontologies into MarkLogic.  These ontologies can be used
to represent various cybersecurity entities.  

# How do I setup ml-cyber?

0) Review gradle.properties to make sure that all parameters are set correctly.

1) ./gradlew mlDeploy

2) ./gradlew importOntologies
    - This step demonstrates the use of MarkLogic Content Pump to ingest the ontologies as triples.
    
3) Open QConsole: http://<host>:8000/qconsole
    - Make sure that database is set to "ml-cyber-content"
    - Top Right Corner there is a menu - Import Workspace - <workspace>/qconsole/ml-cyber.xml
    - This will bring up some sample SPARQL queries

The insert SPARQL statement was defined around the CWE ontology.  
https://cwe.mitre.org/documents/schema/schema_v5.4.2.html
    