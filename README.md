### Hi there 👋

```
@prefix rdf: <http://www.w3.org/1999/02/22-rdf-syntax-ns#> .
@prefix rdfs: <http://www.w3.org/2000/01/rdf-schema#> .
@prefix dcterms: <http://purl.org/dc/terms/> .
@prefix xsd: <http://www.w3.org/2001/XMLSchema#> .
@prefix schema: <http://schema.org/> .
@prefix foaf: <http://xmlns.com/foaf/0.1/> .
@prefix owl: <http://www.w3.org/2002/07/owl#> .
@prefix : <#> . 

<> rdf:type foaf:PersonalProfileDocument .
<> foaf:maker :me .
<> foaf:primaryTopic :me .

:me a schema:Person, foaf:Person ;
  schema:name "Bart Hanssens" ;
  schema:mainEntityOf <>, <https://www.facebook.com/bart.hanssens#>, <https://www.linkedin.com/in/barthanssens#>, <https://twitter.com/BartHanssens#> ;
  owl:sameAs <https://www.facebook.com/bart.hanssens#this>, <https://www.linkedin.com/in/barthanssens#this>, <https://twitter.com/BartHanssens#this> .
  
:this a schema:WebPage, foaf:Document ;
  rdfs:name "Bart Hanssens' Profile Document"@en ;
  dcterms:created "2020-07-12"^^xsd:dateTime ;
  dcterms:creator :me ;
  schema:mainEntity :me ;
  foaf:primaryTopic :me .
```
