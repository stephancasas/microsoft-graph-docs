---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

let requestParameters = {
	select : "id,mail,assignedLicenses",
	filter : "assignedLicenses/any",
};
const result = async () => {
	await graphServiceClient.users.get(requestParameters);
}


```