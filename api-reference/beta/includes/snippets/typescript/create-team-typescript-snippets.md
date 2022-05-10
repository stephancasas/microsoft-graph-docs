---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new TeamRequestBody();
requestBody.additionalData = {
			 ["allowCreateUpdateChannels" , true],
			 ["allowUserEditMessages" , true],
			 ["allowUserDeleteMessages" , true],
			 ["allowGiphy" , true],
			 ["giphyContentRating" , "strict"],
			 ["showInTeamsSearchAndSuggestions" , true],
	 }
async () => {
	await graphServiceClient.groupsById("group-id").team.put(requestBody);
}


```