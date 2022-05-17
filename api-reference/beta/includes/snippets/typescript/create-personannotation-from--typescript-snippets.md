---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new PersonAnnotation();
requestBody.detail = new ItemBody();
requestBody.detail.contentType = BodyType.Text;
requestBody.detail.content = "I am originally from Australia, but grew up in Moscow, Russia.";
requestBody.displayName = "About Me";
const result = async () => {
	await graphServiceClient.me.profile.notes.post(requestBody);
}


```