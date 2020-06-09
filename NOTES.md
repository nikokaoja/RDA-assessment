# Various notes


## Overview of PID

 - Digital Object Identifier (DOI), used to identify literature, data as well as other objects
 - Open Researcher and Contributor ID (ORCID), a persistent identifier for researcher
 - International Geo Sample Number (IGSN), a persistent identifier for physical samples and sample collections
 - Research Organization Registry (ROR), a persistent identifier for organizations
 - Research Resource Identifier (RRID), an identifier for physical resources, such as mice and antibodies, in the Life Sciences


It misses info on metrological aspects of intruments, e.g. calibration/tracebility/uncertainty, etc. unless they are part of the category `Capability`. As stated by the paper authors, reason for not having metrological aspects is the following:

    "As instruments are increasingly complex and specialized, technical metadata, such as configuration and calibration, are often extensive, dynamic, and inherently difficult to standardize. There is no common standard for this kind of technical metadata that would be meaningful for all experiment techniques across scientific disciplines."

A workaround is to use `RelatedIdentifier` to point to the external documentation containing metrological information:
    "Technical metadata may also be linked from the metadata registered with PID infrastructure using RelatedIdentifier with property relationType value HasMetadata to enable automatic retrieval."


Hint: Together with the Sensor Web Enablement (SWE) Common Data Model Encoding Standard, SensorML provides a conceptual model as well as XML and JSON encodings for sensors and measurement processes metadata.


Also, `RelatedIdentifier` could be / should be regularly maintaned to point to the latest digital objects (papers, report, data, workflows) which used the instrument for their generation.

Something 04-CNR.md indicated:

    Moreover, sensor owners require this information to enact semi-automated workflows that execute operations on the sensor instance (such as updating calibration information or accessing the observations collected by a given sensor).

Something from 05-AWI.md indicated:

    Given that platforms and sensors evolve in time (sensors are being calibrated, mounted/unmounted, etc), it is clearly important to trace changes applied to these over time.

Something from 08-ICOS.md indicated:

    At his stage, combining all three steps explained above , we reach the level of “harmonized raw data” which includes in an ideal world a PID for the Hardware, how the hardware has been installed and configured, and how the data collected has been treated (if at all).

Furthermore, say we have a complex instrument which requires careful configuration `RelatedIdentifier` could potentially point to the published configuration of the instrument or maybe not!?

Not sure if `Owner` property actually provides refinement of roles related to the instrument, for example: (1) creator, (2) maintainer, (3) configurator, (4) owner

Probably I would need to make a simple web-page for long-range WindScanner. We should have a default landing page called under
[instruments.windenergy.dtu.dk](instruments.windenergy.dtu.dk) domain.

The above database is an internal development of a system to manage the instrumentation pool (predominately met mast instruments), provide information about the deployed stations, and offer a catalog of responses for different instruments.

We are similar to HZB, we are having custom built and/or pimped commercial instruments, thus we need metadata for Creator as well as Contributor .


Start with DataCite schema, and then checkout ePIC.

Look at NERC vocab of intruments! It could be useful starting point for definitions of instruments.

How do we separate the instrument ownwerhsip from its management.
