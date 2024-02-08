
This Implementation Guide publishes the IHE vocabulary for FormatCode and the IHE managed ValueSet for FormatCode. Given that the FormatCode is contributed to by many IHE domains, this IG is dedicated to the publication and management of the FormatCode vocabulary.

### Technical Overview

FormatCode is a metadata element for identifying the technical format that a document follows. This is related to mimeType, but is more specific to the content requirements than the encoding requirement. Therefore a document following a FormatCode may have many mimeType encodings. The FormatCode is also related to the document type (e.g. LOINC document type), but is more specific to the requirements (constraints) of the content.

The main sections of this IG are:
- [Background](background.html) - provides more detail on what a FormatCode is and how they are maintained
- [The IHE defined Codes](CodeSystem-formatcode.html) - the definition of the codes defined by IHE for use in FormatCode
- [The IHE defined ValueSet](ValueSet-formatcode.html) - the valueset of codes for FormatCode use.

### Download

- [this entire guide](full-ig.zip) 
- the FormatCode CodeSystem and ValueSet in [json](definitions.json.zip), or [xml](definitions.xml.zip)
- The source code for this Implementation Guide can be found on [IHE GitHub repository for FormatCode](https://github.com/IHE/FormatCode)

#### Cross Version Analysis

{% include cross-version-analysis.xhtml %}

#### Dependency Table

{% include dependency-table.xhtml %}

#### IP Statements

{% include ip-statements.xhtml %}

#### Globals

{% include globals-table.xhtml %}
