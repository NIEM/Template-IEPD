# Template IEPD
This is a template IEPD for NIEM 3.0. It is designed to be a starting point for 
IEPD creators. 

IEPDs built from this template should follow the NIEM-MPD 3.0 specification 
located here:
http://reference.niem.gov/niem/specification/model-package-description/3.0/model-package-description-3.0.html

The NIEM-MPD specification defines the contents and structure of IEPDs including 
metadata, XML Schema documents, and documentation.

[![Build Status](https://travis-ci.org/jtmrice/Template-IEPD.svg?branch=master)](https://travis-ci.org/jtmrice/Template-IEPD)

## This template IEPD contatins
1. NIEM schema subset
  http://reference.niem.gov/niem/specification/model-package-description/3.0/model-package-description-3.0.html#section_4.2

  See the NIEM Schema Subset Generation Tool (SSGT) to create a subset for 
  the IEPD based on requirements: http://tools.niem.gov/niemtools/

2. NIEM extension schema
  http://reference.niem.gov/niem/specification/model-package-description/3.0/model-package-description-3.0.html#section_4.3

  An extension schema contains a conformance target identifier as follows:
  ct:conformanceTargets="http://reference.niem.gov/niem/specification/naming-and-design-rules/3.0/#ExtensionSchemaDocument"

3. Catalog file
  http://reference.niem.gov/niem/specification/model-package-description/3.0/model-package-description-3.0.html#section_5.1

4. README
  http://reference.niem.gov/niem/specification/model-package-description/3.0/model-package-description-3.0.html#section_5.4

5. Change Log
  http://reference.niem.gov/niem/specification/model-package-description/3.0/model-package-description-3.0.html#section_5.3

6. Conformance Assertion
  http://reference.niem.gov/niem/specification/model-package-description/3.0/model-package-description-3.0.html#section_5.7
