---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new CloneRequestBody();
requestBody.displayName = "Library Assist";
requestBody.description = "Self help community for library";
requestBody.mailNickname = "libassist";
requestBody.partsToClone = ClonableTeamParts.Apps,tabs,settings,channels,members;
requestBody.visibility = TeamVisibilityType.Public;
async () => {
	await graphServiceClient.teamsById("team-id").clone.post(requestBody);
}


```