Mass assignment can be used to change properties of objects in applications that are not intended to be changed by the authors.

For example, say you capture a request to update a user in Burp that contains the following data:

```json
{
	"firstName": "John",
	"lastName": "Doe"
}
```

You may be able to assign properties that the developers did not intend, like the following.

```json
{
	"firstName": "John",
	"lastName": "Doe",
	"password": "myNewPassword"
}
```

This could be a vector for escalting privileges (change your role), account takeover (change  a password) etc.