# Data Model

## Core

NAMPI-Core, an ontology that describes the basic interactions specified in the
document interpretation act of the
[Factoid Model](https://www.kcl.ac.uk/factoid-prosopography/ontology):
Interactions between authors, sources, locations, and temporal entities, the
content of the interpreted source location. To model this temporal entity in
more detail and enable the system to be better comparable with other data by
default, we chose to limit the shape temporal entities could assume to events as
described in CIDOC-CRM. These events can have a time and a place as well as a
main person and other participants, which can be both persons and groups of
persons. The interactions between participants of such events and the wider
world are modelled as aspects that are used in the events. These aspects are not
defined in particular detail to keep the system as expressive as possible; they
can range from roles within groups and occupations of persons to titles and
names obtained during an event, as well as other things. Thus, the main classes
in NAMPI-Core are: Act (as in document-interpretation-act), Author, Source (and
Source Location), Event, Person, Group, Date, Place, and Aspect. The work on
this ontology is principally complete, but minor changes are being made as
necessary. Detail-ontologies are used to provide this model with more details as
required by individual installations of the NAMPI platform and their
data/research focus.

![Schematic model of the core data](data-scheme.svg)

## Monastic Life

NAMPI-Monastic Life is an ontology describing certain aspects of life in and
related to early modern monasteries. This ontology plays the role of a
detail-ontology as described above, inheriting the main classes and properties
from NAMPI-Core and expanding on them. It describes the various religious
orders, communities, and types of roles in terms of status, occupation,
religious titles, and names. The work on this ontology has been conducted in
parallel to the document interpretation process performed on the sources
included in the project. Due to the fact that the data ingestion process is
still ongoing, the ontology is being expanded continually.

![Overview of the monastic life event data network](mona-network.svg)

## Ontology files

Both ontologies are already publicly available on Github as well as directly
using a persistent URL:

### Ontologies on GitHub

- [Core source repository](https://github.com/nam-pi/core-owl)
- [Monastic life source repository](https://github.com/nam-pi/monastic-life-owl)

### Ontologies with permalink

- [Persistent core ontology file](https://purl.org/nampi/owl/core)
- [Persistent monastic life ontology file](https://purl.org/nampi/owl/monastic-life)

