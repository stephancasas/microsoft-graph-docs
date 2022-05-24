---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new TeamworkTag();
requestBody.displayName = "Finance";
const teamworktagmember = new TeamworkTagMember();
teamworktagmember.additionalData = {
					 "userId" : "92f6952f-61ca-4a94-8910-508a240bc167"
				 }
const teamworktagmember1 = new TeamworkTagMember();
teamworktagmember1.additionalData = {
					 "userId" : "085d800c-b86b-4bfc-a857-9371ad1caf29"
				 }
requestBody.members = [
			teamworktagmember,
			teamworktagmember1
		]
const result = async () => {
	await graphServiceClient.teamsById("team-id").tags.post(requestBody);
}


```