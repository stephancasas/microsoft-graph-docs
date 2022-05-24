---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new AgreementFileLocalization();
requestBody.fileName = "Contoso ToU for guest users (French)";
requestBody.language = "fr-FR";
requestBody.isDefault = false;
requestBody.isMajorVersion = false;
requestBody.displayName = "Contoso ToU for guest users (French)";
requestBody.fileData = new AgreementFileData();
requestBody.fileData.data = btoa("base64JVBERi0xLjUKJb/3ov4KNCAwIG9iago8PCAvTGluZWFyaX//truncated-binary-data");
const result = async () => {
	await graphServiceClient.identityGovernance.termsOfUse.agreementsById("agreement-id").files.post(requestBody);
}


```