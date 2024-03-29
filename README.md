
# Template IEPD

This repo provides templates for different versions of [NIEM IEPDs](https://niem.github.io/reference/iepd/).  This can be used as a starting point for IEPD developers.

The NIEM IEPD specification defines the contents and structure of IEPDs including metadata, XML Schema documents, and documentation.

Version | View | Download | Use with | Specification | Comments
--- | --- | --- | --- | --- | ---
3.0 | [GitHub](https://github.com/NIEM/Template-IEPD/tree/niem-3.0) | [zip](https://github.com/NIEM/Template-IEPD/archive/refs/tags/niem-3.0.zip) | NIEM&nbsp;3.0&#8209;3.2 | [MPD v3.0.1](https://niem.github.io/MPD-Spec/v3.0.1/model-package-description-3.0.1.html) | Initial version of the template.
4.0 | [GitHub](https://github.com/NIEM/Template-IEPD/tree/niem-4.0) | [zip](https://github.com/NIEM/Template-IEPD/archive/refs/tags/niem-4.0.zip) | NIEM 4.0-4.2 | [MPD v3.0.1](https://niem.github.io/MPD-Spec/v3.0.1/model-package-description-3.0.1.html) | Minor changes.  The MPD spec was not updated for NIEM 4.0.  The MPD catalog and the NIEM subset were updated to use the NIEM 4.0 release.
5.0 | [GitHub](https://github.com/NIEM/Template-IEPD/tree/niem-5.0) | [zip](https://github.com/NIEM/Template-IEPD/archive/refs/tags/niem-5.0.zip) | NIEM 5.0-5.2 | [IEPD v5.0](https://niem.github.io/MPD-Spec/v5.0/niem-iepd-spec.html) | The MPD specification was updated to focus specifically on IEPDs.  IEPD catalog updated and additional content added.  Created two kinds of messages (a query and a respond) in the template to demonstrate how an IEPD can represent multiple related exchanges in one package.

## Template contents

- **NIEM subset schemas** ([info](https://niem.github.io/reference/iepd/artifacts/subset-schema/))

  - NIEM subset schemas contain user-selected components from a NIEM release.
  - Use the NIEM [Schema Subset Generation Tool (SSGT)](http://tools.niem.gov/niemtools/) to create a subset for an IEPD based on local requirements.
  - The NIEM subset should also include the `wantlist.xml` file generated by the SSGT so that the subset may be easily reloaded and updated for a future version of the IEPD.

- **NIEM extension schema(s)** ([info](https://niem.github.io/reference/iepd/artifacts/extension-schema/))

  - IEPD extension schemas define the components that are needed for an exchange that are not found in NIEM.
  - NIEM schemas must declare a conformance target indicating which version and rule set of the [NIEM Naming and Design Rules (NDR)](https://niem.github.io/reference/specifications/ndr/) are applicable.  This informs conformance tools which set of NDR Schematron rules should be used for validation.  See [conformance targets](https://niem.github.io/reference/specifications/conformance-targets/) for more.

- **MPD/IEPD Catalog file** ([info](https://niem.github.io/reference/iepd/artifacts/iepd-catalog/))

  - A MPD/IEPD catalog defines metadata for an IEPD.  It includes basic information about the IEPD itself, including point of contact information, information about each message defined by the IEPD, and information about the artifacts in the package.

- **README** ([info](https://niem.github.io/reference/iepd/artifacts/#readme))

  - A ReadMe file is documentation that should describe an IEPD, including such information as its purpose, scope, business value, exchange information, typical senders and receivers, and the artifacts in the IEPD.

- **Change Log** ([info](https://niem.github.io/reference/iepd/artifacts/#change-log))

  - A change log describes the changes applied to an IEPD since its previous version.
  - For the initial version of an IEPD, the change log may simply contain the release date.

- **Conformance Assertion** ([info](https://niem.github.io/reference/iepd/artifacts/#conformance-assertion))

  - A conformance assertion should include information such as if the IEPD is NIEM conformant, list any known issues or exceptions, and describe what tools or processes were used to determine conformance.
  - Check that IEPD extension schemas (XML only) are conformant to the automated NIEM [Naming and Design Rules (NDR)](https://reference.niem.gov/niem/specification/naming-and-design-rules/) using the [Conformance Testing Assistant (ConTesA)](https://tools.niem.gov/contesa/).  A report can be downloaded from the tool and included in the IEPD.
    - Note that ConTesA only checks NIEM conformance of XML schemas, not the entire IEPD itself.
    - Note that all IEPD extension schemas must have a conformance target identifier, as specified above, in order for ConTesA to work.  Without it, ConTesA will not know which specific NDR rule set to use and no rules will be run.
  - Check that the full MPD / IEPD package is conformant to the [MPD / IEPD Specification](https://niem.github.io/reference/specifications/iepd/).  This is a manual process, but Appendix E of the [MPD Specification v3.0](https://reference.niem.gov/niem/specification/model-package-description/3.0.1/model-package-description-3.0.1.html#appendix_E) or [IEPD Specification v5.0](https://niem.github.io/MPD-Spec/v5.0/niem-iepd-spec.html#appendix_E) provide a basic checklist of best practices.  A bigger [IEPD checklist](https://niem.github.io/reference/iepd/lifecycle/assemble-and-document/#iepd-review-checklist) is also available to use for manual conformance reviews.

## Other IEPD resources

- [NIEM 3.0 Example IEPDs and supporting artifacts](https://reference.niem.gov/niem/specification/model-package-description/3.0.1/) are available for further reference.

- The [IEPD section](https://niem.github.io/reference/iepd/) on [niem.github.io](https://niem.github.io) contains information about the IEPD lifecycle, IEPD artifacts, and more.

- NIEM is now offering virtual technical deep-dive training.  Three half-day instructor-led sessions are being offered monthly over Webex.  View or follow [@NIEMconnects](https://twitter.com/NIEMconnects) to sign up for a training session.

- Materials from the new technical deep-dive training are also available on the [NIEM-Training GitHub site](https://github.com/NIEM/NIEM-Training).  Resources include the [training syllabus](https://github.com/NIEM/NIEM-Training/blob/main/NIEM%20Training%20Syllabus.md), the [master training document](https://github.com/NIEM/NIEM-Training/blob/main/Master%20NIEM%20Document/Master%20NIEM%20Training%20Document.md), a [simplified mapping spreadsheet](https://github.com/NIEM/NIEM-Training/tree/main/Master%20NIEM%20Document/Mapping_Spreadsheets), and a sample [Crash Driver IEPD](https://github.com/NIEM/NIEM-Training/tree/main/Crash%20Driver%20IEPD).

- An alternative [mapping spreadsheet](https://niem.github.io/reference/iepd/artifacts/mapping-spreadsheet/), which is also used as a way to submit changes to NIEM releases, is available.
