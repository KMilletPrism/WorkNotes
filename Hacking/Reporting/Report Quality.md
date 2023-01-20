
## First Page

- Use the full client name on the front page of the report
- Instead of using the generic term "Penetration Test", be more specific, for example "External Infrastructure Penetration Test"
- Ensure the version numbers are kept up to date
- Make sure the project reference from JIRA is correct
- If two people have done the test, include both authors


## Second Page

 - In the page header, ensure the company name is included in full, not abbreviated.
 - Be specific in the right hand side of the header as to what type of test has been done, e.g. "External Infrastructure and Web Application Test"
 - Ensure the table of contents is updated correctly
	 - The dates are often not the actual dates of the test. Canopy changes this without people noticing
	 - Ensure all names of testers are listed under the author section
	 - Version information needs to be updated and correct
	 - The FAO section if often incorrect. Ensure the correct name is taken from the SOW
- The full table of contents should be the last thing updated to ensure accuracy


##  Management Summary

- In the introduction of what the test is, the template has often not been updated to include the actual test that has been conducted.
- Don't assume that Canopy is going to fill in <CLIENT_NAME> template details. It often doesn't.  Fill in the name yourself
- Often, the description of the phases completed does not match the title. These should be accurate
- Dates of testing start and end should be accurate
- On the graph to the right, the y-axis should be in whole numbers, not decimals. You can right click and *Format Axes* to change this
- The management summary should mention the phases of the project in the order that they appear in the rest of the report
- There is a lot of copying and pasting in the management summary. If this is done, ensure it is accurate. Often the wrong client name is mentioned or the description does not make sense
- Often the findings themselves are references, but sometimes it is incorrect. It should match what is in the tables and the rest of the report
- Make sure references in the management summary to finding details are accurate. E.g. if SSLv2.0 is not mentioned in the finding, it should not appear in the management summary


## Introduction

- The boilerplate here is often left alone. Ensure it is relevant to the test. It often isn't


## Scope

- Ensure everything from the scope in the SOW is included in here.


## Methodology

- Canopy inclueds all methodologies by default in the Word document. You need to manuall remove the irrelevant ones


## Findings

- Ensure all fields are populated. Category is left blank if you don't use the KB.
- Affecte Components is often left out. Ensure all findings have this field filled
- The description should not include specific details of the test. This should be in the details section
- Recommendations need to be relevant
- Update template text that is included in the finding and ensure it is relevant to the specific instance of the issue you are talking about
- Make sure all liks included in Further Information etc. are still active
- If there are links to OWASP etc. ensure that it is pointing to the most up to date version
- When you're saying that a version is "outdated and vulnerable", you need to be specific about what it is vulnerable to
- Ensure all images are centered, have captions and are sized appropriately to fit on the page
- Ensure screenshots are legible as they must be of use to the client
- Ensure evidence is complete - For example ensure evidence of a successful request is included after a screenshot of an intruder brute force


## General Advice

- Ensure formatting is correct. E.g spacing. In Canopy you need to include two spaces between paragraphs if you want a space to appear in the Word document.
- Ensure advice like "Review as soon as possible" should be relevant to the report. If the finding being spoken about is of low severity, there should not be a high sense of urgency in the advice given in management summaries or the finding text. These should be changed from the template if necessary
- Templates are not fixed. The only things in template reports that will never change are Prism branding and legal notices etc. Antyhing in a finding template should be reviewed and changed if not applicable to the specific text
- When referencing things with acronyms like XSS or SQLi, ensure you have included the full name at the start before you begin to refer to it by its abbreviation
- Be specific in finding text. "XSS was found on application functionality" is too vague. What finctionality? Text like "XSS can be used to steal session cookies" should only be included if this was possible with this test
- Keep an eye out for template text not being relevant in summary sections. E.g. "The tables below..." is not relevant if there is only one table and should be changed
- Ensure references in tables are accurate. Canopy assumes references across phases should continue by incrementing the decimal. Phases should actually have different whole number references and do in the Navigation pane on the left. Ensure these references match.
- Ensure summary / remediation advice is relevant to the specific finding. E.g. dont talk about ensuring hashing algorithms are strong if hashing isn't the specific cryptography issue in the finding
- The summary should be remmediation advice. Text like "The application allows user enumeration" is not advice, and should be changed.
- Esure severity levels match CVSS3 scores
- Text should have the same font and size across the document. Sometimes Canopy changes formatting and this needs to be fixed in the Word document
- Remove all hyperlinks from the document
- Ensure there is no unnecessary whitespace between sections