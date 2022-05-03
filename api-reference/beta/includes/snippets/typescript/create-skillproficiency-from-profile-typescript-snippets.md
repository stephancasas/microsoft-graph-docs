---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new SkillProficiency();
requestBody.categories = [
			"Professional"
		]
requestBody.allowedAudiences = AllowedAudiences.Organization;
requestBody.displayName = "API Design";
requestBody.proficiency = SkillProficiencyLevel.GeneralProfessional;
requestBody.collaborationTags = [
			"ableToMentor"
		]
const result = async () => {
	await graphServiceClient.me.profile.skills.post(requestBody);
}


```