# Persistent Identification of Instruments

In this document we will first review and then apply the Research Data Alliance (RDA) Working Group (WG) Persistent Identification of Instruments (PIDINST) output to the wind energy related instrumentation.

## Review of PIDINST output
As stated in the [paper](https://datascience.codata.org/articles/10.5334/dsj-2020-018/):

    "Instruments play an essential role in creating research data. Given the importance of instruments and associated metadata to the assessment of data quality and data reuse, globally unique, persistent and resolvable identification of instruments is crucial. "

By instrument, it was meant *measuring instrument*, which is defined by [VIM](https://www.bipm.org/utils/common/documents/jcgm/JCGM_200_2012.pdf) as:

    "a device used for making measurements, alone or in conjunction with one or more supplementary devices"


Accordingly, PIDINST WG developed a community-driven solution for persistent identification of instruments. Their initial work was based on 14 use cases which were assesses and a PIDINST metadata schema derived. The schema was prototyped using [DataCite](https://datacite.org/) and [ePIC](https://www.pidconsortium.net/).

The PID schema contains following instrument properties:

- Identification
- Instrument
- Model
- Owner
- Manufacturer
- Date
- Capability
- Output
- Related Instrument



The majority of the use cases (60%) originated from Earth Sciences domain. Since wind energy domain partially belongs to Earth Sciences domain it represents a strong candidate for the application of the PIDINST in terms of a direct reuse of the existing examples, especially those provided by ICOS ESFRI (Use Case no 8 in the [paper](https://datascience.codata.org/articles/10.5334/dsj-2020-018/)).

## Adoption of PIDINST schema - WindScanner user case

### Introduction to domain

### Introduction to infrastructure

### PIDINST implementation