---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new AccessPackageResourceRequest();
requestBody.catalogId = "26ac0c0a-08bc-4a7b-a313-839f58044ba5";
requestBody.requestType = "AdminAdd";
requestBody.justification = "";
requestBody.accessPackageResource = new AccessPackageResource();
requestBody.accessPackageResource.displayName = "Faculty cafeteria ordering";
requestBody.accessPackageResource.description = "Example application";
requestBody.accessPackageResource.url = "https://myapps.microsoft.com/example.com/signin/Faculty%20cafeteria%20ordering/f1e3b407-942d-4934-9a3f-cef1975cb988/";
requestBody.accessPackageResource.resourceType = "Application";
requestBody.accessPackageResource.originId = "2f1099a6-d4fc-4cc9-a0ef-ddd3f1bf0b7e";
requestBody.accessPackageResource.originSystem = "AadApplication";
const accesspackageresourceattribute = new AccessPackageResourceAttribute();
accesspackageresourceattribute.additionalData = {
						 "attributeName" : "extension_2b676109c7c74ae2b41549205f1947ed_personalTitle",
						 "isEditable" : true,
						 "isPersistedOnAssignmentRemoval" : true,
							 ["@odata.type" , "#microsoft.graph.accessPackageResourceAttributeQuestion"],
								 ["@odata.type" , "#microsoft.graph.accessPackageTextInputQuestion"],
								 ["isRequired" , false],
								 ["sequence" , 0],
								 ["isSingleLineQuestion" , true],
									 ["defaultText" , "Title"],
									 ["localizedTexts" , [
										]
							 ["@odata.type" , "#microsoft.graph.accessPackageUserDirectoryAttributeStore"],
					 }
requestBody.accessPackageResource.attributes = [
				accesspackageresourceattribute
			]
const result = async () => {
	await graphServiceClient.identityGovernance.entitlementManagement.accessPackageResourceRequests.post(requestBody);
}


```