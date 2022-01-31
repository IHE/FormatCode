# FormatCode
IG to manage the FormatCode vocabulary

continuous build available at http://build.fhir.org/ig/IHE/FormatCode/branches/master/index.html

formal canonical URI for the IHE code system `http://ihe.net/fhir/ihe.formatcode.fhir/CodeSystem/formatcode`

formal publication URL http://profiles.ihe.net/fhir/ihe.formatcode.fhir/index.html

# Instructions to IHE authors on requesting changes to the FormatCode vocabulary

With the publication of the IHE FormatCode Implementation Guide (this content), the formal management of the IHE authored FormatCode vocabulary has moved. The previous wiki page is no longer formal, and will be retired.

Acceptable Changes:
* Creation of a new code -- even experimental codes can be added. However the intention would be that the new code is intended to be a normative code. Thus please do not propose the addition of temporary, or project specific codes. The codes published here are formal publication of IHE.
* Update of a code description
  * note that once a code has been used it must go through the proper code lifecycle. If a committee needs a code changed, this is accomplished by deprecating the old one and creating a new one
* Deprecating a code

## Submission Process

1. The committee that is requesting the change must have formal governance approval for the change. 
2. Create an Issue identifying the need for the change
3. The committee designated author (anyone with the authority of the committee) will prepare a Github "Pull-Request" by creating a branch. The subsequent steps will occur within your branch.
4.  Edit the codesystem-formatcode.xml
  * to add your new concepts, within your domain group
  * update CodeSystem.date to the date of your edit
5. Edit the Bundle-history-IHE-formatcode.codesystem.xml to add a new Provenance record explaining the change. Within the new entry:
  * Indicate the dates of the change - YYYY, MM, and DD represent the year, month and date of the change (always 4-digit, and 2-digit, respectively)
      * The fullUrl is in the format "urn:oid:1.3.6.1.4.1.19376.1.2.3.1.YYYYMMDD"
      * The value of Provenance.id is in the format "formatcode-provenance-YYYYMMDD"
      * The value of Provenance.occuredPeriod.end is in the format "YYYY-MM-DD"
      * The value of Provenance.recorded is in the format "YYYY-MM-DDT13:00:00.0000Z"
  * Indicate the reason for the change, be specific but keep to a sentence. Might include CP number if you want.  
  * Indicate who the committee designated author is
  * Indicate what domain is the custodian of that code
6. Edit the implementationguide-IHE.FormatCode.xml to update the ImplementationGuide.date of this change, and increment ImplementationGuide.version
7. Create a Pull-Request with the branch containing your changes and indicate that it closes your new Issue.
  
If you have any problems, or need assistance contact JohnMoehrke@gmail.com or the assigned Librarian of the FormatCode IG.
  
# TODO

* register this vocabulary with fhir terminology -- John is working with HTA
