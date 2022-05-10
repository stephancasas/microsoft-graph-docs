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
							"8a256a2b-b617-496d-b51b-e76466e88db0"
						]
					 "skuId" : "84a661c4-e949-4bd2-a560-ed7766fcaf2b"
				 }
const assignedlicense1 = new AssignedLicense();
assignedlicense1.additionalData = {
					 "disabledPlans" : [
						]
					 "skuId" : "f30db892-07e9-47e9-837c-80727f46fd3d"
				 }
requestBody.addLicenses = [
			assignedlicense,
			assignedlicense1
		]
requestBody.removeLicenses = [
		]
const result = async () => {
	await graphServiceClient.me.assignLicense.post(requestBody);
}


```