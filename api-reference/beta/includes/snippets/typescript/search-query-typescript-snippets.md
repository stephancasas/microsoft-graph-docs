---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new QueryRequestBody();
const searchrequest = new SearchRequest();
searchrequest.additionalData = {
					 "entityTypes" : [
							"externalItem"
						]
					 "contentSources" : [
							"/external/connections/connectionfriendlyname"
						]
						 ["queryString" , "contoso product"],
					 "from" : 0,
					 "size" : 25,
					 "fields" : [
							"title",
							"description"
						]
				 }
requestBody.requests = [
			searchrequest
		]
const result = async () => {
	await graphServiceClient.search.query.post(requestBody);
}


```