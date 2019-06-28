---
layout: default
---

## Description

```turtle

@prefix : <https://www.gdelt.stream/stream#> .
@prefix dcat: <http://www.w3.org/ns/dcat#> .
@prefix owl: <http://www.w3.org/2002/07/owl#> .
@prefix rdf: <http://www.w3.org/1999/02/22-rdf-syntax-ns#> .
@prefix xml: <http://www.w3.org/XML/1998/namespace> .
@prefix xsd: <http://www.w3.org/2001/XMLSchema#> .
@prefix rdfs: <http://www.w3.org/2000/01/rdf-schema#> .
@prefix vocals: <http://w3id.org/rsp/vocals#> .
@prefix vprov: <http://w3id.org/rsp/vocals-prov#> .
@prefix vsd: <http://w3id.org/rsp/vocals-sd#> .
@prefix dcat: <http://www.w3.org/ns/dcat#> .
@prefix time: <http://www.w3.org/2006/time#> .
@prefix frmt: <http://www.w3.org/ns/formats/> .
@prefix prov: <http://www.w3.org/ns/prov#> .

```
## Schema


## Sample Data

## Example Input

|           |          |        |      |           |     |                |     |   |   |   |   |     |   |   |   |   |   |   |   |   |   |   |   |   |   |     |     |    |   |      |    |   |    |                   |   |                                        |    |      |       |         |          |         |   |   |   |   |   |   |   |   |   |                                        |    |      |       |         |          |         |                |                                                                                                                                 |
|-----------|----------|--------|------|-----------|-----|----------------|-----|---|---|---|---|-----|---|---|---|---|---|---|---|---|---|---|---|---|---|-----|-----|----|---|------|----|---|----|-------------------|---|----------------------------------------|----|------|-------|---------|----------|---------|---|---|---|---|---|---|---|---|---|----------------------------------------|----|------|-------|---------|----------|---------|----------------|---------------------------------------------------------------------------------------------------------------------------------|
| 835209455 | 20180401 | 201804 | 2018 | 2018.2493 | GOV | STATE OFFICIAL |     |   |   |   |   | GOV |   |   |   |   |   |   |   |   |   |   |   |   | 1 | 020 | 020 | 02 | 1 | 3.0  | 3  | 1 | 3  | 1.3986013986014   | 3 | Raleigh, North Carolina, United States | US | USNC | NC183 | 35.7721 | -78.6386 | 1024242 | 0 |   |   |   |   |   |   |   | 3 | Raleigh, North Carolina, United States | US | USNC | NC183 | 35.7721 | -78.6386 | 1024242 | 20190401203000 | http://www.reflector.com/National-News/2019/04/01/With-Congress-seat-in-grasp-NC-urges-census-participation.html                |
| 835209456 | 20180401 | 201804 | 2018 | 2018.2493 | GOV | STATE OFFICIAL |     |   |   |   |   | GOV |   |   |   |   |   |   |   |   |   |   |   |   | 1 | 020 | 020 | 02 | 1 | 3.0  | 1  | 1 | 1  | 1.3986013986014   | 2 | North Carolina, United States          | US | USNC |       | 35.6411 | -79.8431 | NC      | 0 |   |   |   |   |   |   |   | 3 | Raleigh, North Carolina, United States | US | USNC | NC183 | 35.7721 | -78.6386 | 1024242 | 20190401203000 | http://www.reflector.com/National-News/2019/04/01/With-Congress-seat-in-grasp-NC-urges-census-participation.html                |
| 835209457 | 20180401 | 201804 | 2018 | 2018.2493 | GOV | STATE OFFICIAL |     |   |   |   |   | GOV |   |   |   |   |   |   |   |   |   |   |   |   | 1 | 020 | 020 | 02 | 1 | 3.0  | 6  | 1 | 6  | 1.3986013986014   | 2 | North Carolina, United States          | US | USNC |       | 35.6411 | -79.8431 | NC      | 0 |   |   |   |   |   |   |   | 2 | North Carolina, United States          | US | USNC |       | 35.6411 | -79.8431 | NC      | 20190401203000 | http://www.reflector.com/National-News/2019/04/01/With-Congress-seat-in-grasp-NC-urges-census-participation.html                |
| 835209458 | 20180401 | 201804 | 2018 | 2018.2493 | LEG | CONGRESS       |     |   |   |   |   | LEG |   |   |   |   |   |   |   |   |   |   |   |   | 1 | 120 | 120 | 12 | 3 | -4.0 | 1  | 1 | 1  | -3.41880341880341 | 1 | Mexico                                 | MX | MX   |       | 23      | -102     | MX      | 0 |   |   |   |   |   |   |   | 2 | Florida, United States                 | US | USFL |       | 27.8333 | -81.717  | FL      | 20190401203000 | http://www.island-reporter.com/page/content.detail/id/587193/Citing-constitutional-concerns--Rooney-votes-to-override-veto.html |
| 835209459 | 20180401 | 201804 | 2018 | 2018.2493 | USA | MISSISSIPPI    | USA |   |   |   |   |     |   |   |   |   |   |   |   |   |   |   |   |   | 0 | 040 | 040 | 04 | 1 | 1.0  | 10 | 1 | 10 | -1.48698884758364 | 2 | Mississippi, United States             | US | USMS |       | 32.7673 | -89.6812 | MS      | 0 |   |   |   |   |   |   |   | 2 | Mississippi, United States             | US | USMS |       | 32.7673 | -89.6812 | MS      | 20190401203000 | http://www.jacksonfreepress.com/news/2019/apr/01/reeves-skipping-first-debate-governor-despite-earl/                            |


## Mappings

## Converted Data

## SGraph

```turtle
<http://gdelt.stream/events> a vocals:StreamDescriptor , vsd:CatalogService ;
	dcat:dataset <http://localhost:80/mentions>  .

<http://gdelt.stream/events> a vocals:Stream ;
        dcat:title "GDELT Events Stream"^^xsd:string ;
        dcat:publisher <http://www.streamreasoning.org> ;
        dcat:description "GDELT Events Stream"^^xsd:string ;
        vocals:windowType vocals:logicalTumbling ;
        vocals:windowSize "PT15M"^^xsd:duration ;
        vocals:hasEndpoint [
                 a vocals:StreamEndpoint ;
                 dcat:license <https://creativecommons.org/licenses/by-nc/4.0/> ;
                 dcat:format frmt:JSON-LD;
                 dcat:accessURL "ws://gdelt.stream/events" ];

.

```