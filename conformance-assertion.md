
# IEPD Conformance Assertion

> The following is a sample conformance assertion.  Update the text to reflect actual assertions and tools used, notes, known issues, and any other information that might be helpful for users.

IEPD conformance was reviewed by NAME on DATE.

## Specifications

This IEPD conforms to the following NIEM specifications:

- [NIEM Naming and Design Rules (NDR), version 5.0](https://reference.niem.gov/niem/specification/naming-and-design-rules/5.0/niem-ndr-5.0.html)
  - All XML schemas and instances are well-formed and pass basic validation tests, as tested by Oxygen.
  - NDR conformance of the NIEM subset schemas is asserted due to the use of the [SSGT](https://niem.github.io/reference/tools/ssgt/) to generate the subset.
  - The extension schema was tested for NDR conformance using [NDR Schematron rules in Oxygen](https://niem.github.io/reference/tools/oxygen/ndr/) during development and [ConTesA](https://niem.github.io/reference/tools/contesa/) to review and generate the final report.  All checks pass, with the exception listed below.

- [NIEM Information Exchange Package Description (IEPD), version 5.0](https://reference.niem.gov/niem/specification/model-package-description/5.0/niem-iepd-spec-5.0.html)
  - The IEPD catalog (iepd-catalog.xml) is valid against the [IEPD catalog schema](https://reference.niem.gov/niem/specification/model-package-description/5.0/iepd-catalog-schema/iepd-catalog.xsd).
  - This IEPD follows the guidance provided by [Appendix E. Guidance for IEPD Directories (non-normative)](https://niem.github.io/MPD-Spec/v5.0/niem-iepd-spec.html#appendix_E) in the IEPD specification.
  - The IEPD passes the checks listed in the [IEPD review checklist](https://niem.github.io/reference/iepd/lifecycle/assemble-and-document/#iepd-review-checklist).

- [NIEM Conformance Targets Attribute Specification (CTAS), version 3.0](https://reference.niem.gov/niem/specification/conformance-targets-attribute/3.0/NIEM-CTAS-3.0-2014-07-31.html)
  - The IEPD extension schema includes the schema-level `conformanceTargets` attribute as described by this specification.

- [NIEM Conformance Specification, version 5.0](https://reference.niem.gov/niem/specification/conformance/5.0/niem-conformance-spec-5.0.html)
  - IEPD schemas and sample instances conform to the Naming and Design Rules Specification, version 5.0.
  - The IEPD itself conformance to the IEPD Specification, version 5.0.
  - The IEPD maintains semantic integrity with NIEM by avoiding duplication and reusing content from the NIEM release where applicable and following [NIEM conformance practices](https://niem.github.io/reference/specifications/conformance/).

## Additional notes

- Business requirements associated with the information exchange defined by this IEPD were verified by the author and by subject matter experts.
- The sample IEPD was manually reviewed to ensure that all data requirements have been successfully maintained and represented.

## Known issues

Naming and Design Rules (NDR) conformance validation was completed using the NDR Schematron rules in the Oxygen XML editor.  All errors and warnings were resolved with the exception of the use of XML comments that were purposefully left in place to help guide IEPD developers when reviewing this IEPD in the future. All XML comments can be removed at any time for full NDR conformance, however their presence has no effect on the functionality of the IEPD.
