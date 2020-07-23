# FormatCode
IG to manage the FormatCode vocabulary

continuous build available at http://build.fhir.org/ig/IHE/FormatCode/branches/master/index.html

formal canonical URI http://profiles.ihe.net/fhir/iti.formatcode.fhir

formal publication URL http://profiles.ihe.net/fhir/iti.formatcode.fhir/index.html

# Instructions to IHE authors on requesting changes to the FormatCode vocabulary
With the publication of the IHE FormatCode Implementation Guide (this content), the formal management of the IHE authored FormatCode vocabulary has moved. The previous wiki page is no longer formal, and will be retired.

Acceptable Changes:
* Creation of a new code -- even experimental codes can be added. However the intention would be that the new code is intended to be a normative code. Thus please do not propose the addition of temporary, or project specific codes. The codes published here are formal publication of IHE.
* Update of a code description
  * note that once a code has been used it must go through the proper code lifecycle. If a committee needs a code changed, this is accomplished by deprecating the old one and creating a new one
* Deprecating a code

1. The committee that is requesting the change must hve formal governance approval for the change. 
2. The committee designated author (anyone with the authority of the committee) will prepare a GIT "Pull-Request"
  a. Edit the codesystem-formatcode.xml to add your new concepts
  b. Edit the codesystem-formatcode.xml date to the date of your edit
  c. Edit the provenance-IHE-formatcode.codesystem.xml to add a new Provenance record explaining the can
    * Indicate the dates of the change
    * Indicate the reason for the change  
    * Indicate who the committee designated author is
    * Indicate what domain is the custodian of that code	
  d. Edit the implementationguide-IHE.FormatCode.xml to update the date of this change, and version increment
  
  If you have any problems, or need assistance contact JohnMoehrke@gmail.com or the assigned Librian of the FormatCode IG.
  
  # TODO
* formal approval of this publication system (IG vs the wiki)
* publish on IHE http://profiles.ihe.net/ITI/FormatCode 
* register this IG with fhir IG registry
* register this vocabulary with fhir terminology

# DONE
* Should I add to the concepts that moved to HL7 the extension replacedBy
* use IHE template -- which does work locally, but not available yet on the HL7 build machine
* Define codeSystem and valueSet with original IHE OIDs but place them into THIS IG, not MHD as they are broader than MHD
* Get all domain FormatCodes included
* Include as comment the CDA template associated with the FormatCode
