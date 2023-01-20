Web scoping calls can be conducted by asking the client the following questions:

- How many URLs?
- How many user roles ?
- Any APIs that drive the application's functionality ?
	- Is there a separate API test being planned that is actually the same API?
- How many unique webpages
- What types of user roles are there and which ones are we being given?
- Technologies used to build it ?
- Staging or Prod Environment ?
- WAF in place ? Do we need whitelisting ? E.g Cloudflare
- The nature of the webapp , most business-critical functionalities ?
- Phase ? Number of Days ?
- Anything in particular that should not be included in scope and tested?
- If there are different roles for the application, are they all using the same portal (URL) or are they separate?
	- Is this a test environment? Can you easily reset data? Our scans at POST endpoints may create many objects