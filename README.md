# FormatCode
IG to manage the FormatCode vocabulary

continuous build available at http://build.fhir.org/ig/IHE/FormatCode/branches/master/index.html

formal canonical URI http://ihe.net/fhir/ihe.formatcode.fhir/CodeSystem/formatcode

formal publication URL http://profiles.ihe.net/fhir/ihe.formatcode.fhir/index.html

# Instructions to IHE authors on requesting changes to the FormatCode vocabulary

With the publication of the IHE FormatCode Implementation Guide (this content), the formal management of the IHE authored FormatCode vocabulary has moved. The previous wiki page is no longer formal, and will be retired.

Acceptable Changes:
* Creation of a new code -- even experimental codes can be added. However the intention would be that the new code is intended to be a normative code. Thus please do not propose the addition of temporary, or project specific codes. The codes published here are formal publication of IHE.
* Update of a code description
  * note that once a code has been used it must go through the proper code lifecycle. If a committee needs a code changed, this is accomplished by deprecating the old one and creating a new one
* Deprecating a code

## Submission Process

1. The committee that is requesting the change must hve formal governance approval for the change. 
2. Create an Issue identifying the need for the change
3. The committee designated author (anyone with the authority of the committee) will prepare a GIT "Pull-Request"
4.  Edit the codesystem-formatcode.xml 
  * to add your new concepts, within your domain group
  * update .date to the date of your edit
5. Edit the Bundle-history-IHE-formatcode.codesystem.xml to add a new Provenance record explaining the change
  * Indicate the dates of the change
  * Indicate the reason for the change, be specific but keep to a sentence. might include CP number if you want.  
  * Indicate who the committee designated author is
  * Indicate what domain is the custodian of that code	
6. Edit the implementationguide-IHE.FormatCode.xml to update the date of this change, and version increment
7. Create a Pull-Request with your changes and indicate that it closes your new Issue.
  
If you have any problems, or need assistance contact JohnMoehrke@gmail.com or the assigned Liberian of the FormatCode IG.
  
# TODO

* register this vocabulary with fhir terminology -- John is working with HTA

# DONE

* formal approval from IHE to publish July 24, 2020
* Should I add to the concepts that moved to HL7 the extension replacedBy
* use IHE template -- which does work locally, but not available yet on the HL7 build machine
* Define codeSystem and valueSet with original IHE OIDs but place them into THIS IG, not MHD as they are broader than MHD
* Get all domain FormatCodes included
* Include as comment the CDA template associated with the FormatCode
* publish on IHE http://profiles.ihe.net/ITI/FormatCode 
* get canonical URI http://ihe.net/fhir/ihe.formatcode.fhir/CodeSystem/formatcode redirected for HTML mime-type to http://profiles.ihe.net/ITI/FormatCode
* update the IHE wiki page to indicate the change of policy
* update the IHE wiki where other pages point at the FormatCode wiki page (such as on the XDS profile page)
* Added in to the ValueSet the codeSystem from HL7 with their codes
* register this IG with fhir IG registry 
