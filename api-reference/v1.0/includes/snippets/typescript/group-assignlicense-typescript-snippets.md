---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new AssignLicenseRequestBody();
const assignedlicense = new AssignedLicense();
assignedlicense.additionalData = {
					 "disabledPlans" : [
							"113feb6c-3fe4-4440-bddc-54d774bf0318",
							"14ab5db5-e6c4-4b20-b4bc-13e36fd2227f"
						]
					 "skuId" : "b05e124f-c7cc-45a0-a6aa-8cf78c946968"
				 }
const assignedlicense1 = new AssignedLicense();
assignedlicense1.additionalData = {
					 "disabledPlans" : [
							"a413a9ff-720c-4822-98ef-2f37c2a21f4c"
						]
					 "skuId" : "c7df2760-2c81-4ef7-b578-5b5392b571df"
				 }
requestBody.addLicenses = [
			assignedlicense,
			assignedlicense1
		]
requestBody.removeLicenses = [
		]
const result = async () => {
	await graphServiceClient.groupsById("group-id").assignLicense.post(requestBody);
}


```