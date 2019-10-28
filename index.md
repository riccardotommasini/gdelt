---
layout: default
---

# GDELT Project Description

The Global Database of Events, Language & Tone [ (GDELT) project] (www.gdeltproject.org)
is a family of vast and heterogeneous Web Streams that is considered as the largest
open-access spatio-temporal archive for human society. Its Global Knowledge Graph spans
more than 215 years and connects people, organizations, locations, all over the world.
In particular, GDELT complex from a complex domain. It captures themes, images, and emotions
into a single holistic global network. GDELT data can be accessed via Google Big Query or via
a number APIs that run pre-defined analyses. Therefore, the interested researches are forced
to either run their analysis via the pay-per-use service or stick with the provided APIs.

# ISWC Poster Paper

[Download Preprint](./assets/pdf/poster464.pdf)
# Publication Guidelines

![Branching](./assets/images/lc.png)

## Step 0 - Naming Things

We designed GDELT Stream URIs accordingly to [W3C recommendations](https://www.w3.org/TR/cooluris/#cooluris).

-  http://gdelt.stream/vocab# refers to GDELT native vocabulary (e.g. gdelt:Event, gdelt:Mention)
-  http://gdelt.stream/onto/cameo# refers to the OWL 2 version of the CAMEO ontology
-  http://gdelt.stream/onto/gcam# refers to the OWL 2 version of the GCAM ontology

-  http://gdelt.stream/ist/ refers to individual instances, e.g. an Actor or an Event
-  http://gdelt.stream/time refers to time instants


## Step 1 - Modeling the Domain




[CAMEO Ontology OWL File](./assets/ontologies/cameo.owl)

## Step 2 - Describe the Stream

We used VoCaLS to describe GDELT streams. Listing 1.1 shows an example of description for the
GDELT Event Stream. In
VoCaLS, a Web Stream is represented using vocals:Stream,
i.e., an unbounded sequence
of data items that might be
accessible on the Web. A
vocals:StreamDescriptor, i.e,
a HTTP-accessible document
that contains stream metadata. Finally, the stream content can be consumed
via a vocals:StreamEndpoint, that refer to actual sources using dcat:accessURL
property. GDELT does not use a licence format, thus we include a licence that
is compliant with the terms of use.

## Step 3 -  Annotate and Covert





## Step 4 - Publish the Stream

The unbounded nature of Streaming Linked Data makes it impossible to
directly add a data stream to the LOD Cloud [9, 7]. However, using an RSP
Engine that focus on RDF Stream provisioning like TripleWave [7], one can
publish a stream describing useing VoCaLS. TripleWave relises on Barbieri et
al’s vision [2] of serving a ”static” named graph called S-Graph via REST API,
to identify and describe the streams. Moroever, they envisioned that the stream
elements an RDF Graph are called I-Graphs. We shared the VoCALS description
files like the one in Listing 1.1 as S-GRAPH via REST APIs. Since the concept of
event is first-class, we opted for a graph-based stream data model that maintains
the granularity of information.


Code to run a local version of GDELT RDF Stream can be found [here](https://www.dropbox.com/s/i3nlitlh9e9nqyh/webstreams.zip?dl=0)
A comprehensive guide to how to build and run the code above is available [here](https://www.dropbox.com/s/7j2r7x5h91zpbiq/README.md?dl=0)

Alternatively, GDELT RDF Streams mirrors can be run using docker


‘‘‘

docker run -p 8080:8080 -p 80:80 streamreasoning/webstreams_gdelt_{name}

‘‘‘

name:
    - events
    - mentions
    - gkg

# GDELT Streams


- [Event Stream](./events-stream.html).
- [Mentions Stream](./mentions-stream.html).
- [GKG Stream](./gkg-stream.html).
