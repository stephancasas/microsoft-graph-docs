---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new ReplyRequestBody();
requestBody.post = new Post();
requestBody.post.body = new ItemBody();
requestBody.post.body.contentType = BodyType.Html;
requestBody.post.body.content = "<html><body><div><div><div><div>When and where? </div></div></div></div></body></html>";
const extension = new Extension();
extension.additionalData = {
						 "@odata.type" : "microsoft.graph.openTypeExtension",
						 "extensionName" : "Com.Contoso.HR",
						 "companyName" : "Contoso",
						 "expirationDate" : "2015-07-03T13:04:00.000Z",
						 "topPicks" : [
								"Employees only",
								"Add spouse or guest",
								"Add family"
							]
					 }
requestBody.post.extensions = [
				extension
			]
async () => {
	await graphServiceClient.groupsById("group-id").threadsById("conversationThread-id").postsById("post-id").reply.post(requestBody);
}


```