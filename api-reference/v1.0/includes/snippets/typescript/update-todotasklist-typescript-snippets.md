---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new TodoTaskList();
requestBody.displayName = "Vacation Plan";
const result = async () => {
	await graphServiceClient.me.todo.listsById("todoTaskList-id").patch(requestBody);
}


```