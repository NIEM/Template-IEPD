# Template IEPD

This is a template IEPD for NIEM 4.0. It is designed to be a starting point for IEPD creators.

IEPDs built from this template should follow the [NIEM-MPD 3.0.1 specification](https://reference.niem.gov/niem/specification/model-package-description/3.0.1/model-package-description-3.0.1.html)

The NIEM-MPD specification defines the contents and structure of IEPDs including metadata, XML Schema documents, and documentation.

[Example IEPDs and supporting artifacts](https://reference.niem.gov/niem/specification/model-package-description/3.0.1/) are available for further reference.

[![Build Status](https://travis-ci.org/NIEM/Template-IEPD.svg?branch=master)](https://travis-ci.org/NIEM/Template-IEPD)

## This template IEPD contains

1. [NIEM schema subset](http://reference.niem.gov/niem/specification/model-package-description/3.0.1/model-package-description-3.0.1.html#section_4.2)

    - See the [NIEM Schema Subset Generation Tool (SSGT)](http://tools.niem.gov/niemtools/) to create a subset for the IEPD based on local requirements

2. [NIEM extension schema](http://reference.niem.gov/niem/specification/model-package-description/3.0.1/model-package-description-3.0.1.html#section_4.3)

    - An extension schema contains a conformance target identifier in the schema declaration as follows:

      ```ct:conformanceTargets="http://reference.niem.gov/niem/specification/naming-and-design-rules/3.0/#ExtensionSchemaDocument"```

3. [Catalog file](http://reference.niem.gov/niem/specification/model-package-description/3.0.1/model-package-description-3.0.1.html#section_5.1)

    - See [mpd-catalog-3.0.xsd](https://reference.niem.gov/niem/specification/model-package-description/3.0.1/xsd-mpd-catalog/mpd-catalog-3.0.xsd) for the XML Schema that defines this file.

4. [README](http://reference.niem.gov/niem/specification/model-package-description/3.0.1/model-package-description-3.0.1.html#section_5.4)

5. [Change Log](http://reference.niem.gov/niem/specification/model-package-description/3.0.1/model-package-description-3.0.1.html#section_5.3)

6. [Conformance Assertion](http://reference.niem.gov/niem/specification/model-package-description/3.0.1/model-package-description-3.0.1.html#section_5.7)

    - See the [Conformance Testing Assistant (ConTesA)](https://tools.niem.gov/contesa/) to test automated [NDR](https://reference.niem.gov/niem/specification/naming-and-design-rules/) rules on IEPD extension schemas and to generate a conformance assertion.
    - Note that all local NIEM extension schemas must have a conformance target identifier as specified above in order for the NDR rules to be applied.
