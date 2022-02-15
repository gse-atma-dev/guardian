# Import a Policy

### IMPORT A POLICY

**Description**: Imports new policy and all associated artifacts from IPFS into the local DB. Only users with the Root Authority role are allowed to make the request.

**Policy import (unzip content)**

`POST /api/v1/policies/import/preview`

**Request:**

.zip file

**Response body:**

```
{
	"policy":{
		...
	},
	"tokens":[
		...
	],
	"schemas":[
		...
	]
}
```

****

**Policy import**

`POST /api/v1/policies/import`

**Request body:**

```
{
	//Put the response from the step 5 here
}
```

****

**Publish of the imported policy**

`PUT /api/v1/policies/61dd9f1ae2becb0015685bfa/publish`

**Request body:**

`{"policyVersion":"1.0.0"}`