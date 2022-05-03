---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new Contact();
requestBody.parentFolderId = "parentFolderId-value";
requestBody.birthday =  new Date("datetime-value");
requestBody.fileAs = "fileAs-value";
requestBody.displayName = "displayName-value";
requestBody.givenName = "givenName-value";
requestBody.initials = "initials-value";
const result = async () => {
	await graphServiceClient.me.contactFoldersById("contactFolder-id").contacts.post(requestBody);
}


```