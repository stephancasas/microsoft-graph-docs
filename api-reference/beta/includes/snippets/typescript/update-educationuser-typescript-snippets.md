---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new EducationUser();
const relatedcontact = new RelatedContact();
relatedcontact.additionalData = {
					 "displayName" : "Father Time",
					 "emailAddress" : "father@time.com",
					 "mobilePhone" : "4251231234",
					 "relationship" : "guardian",
					 "accessConsent" : true
				 }
const relatedcontact1 = new RelatedContact();
relatedcontact1.additionalData = {
					 "displayName" : "Mother Nature",
					 "emailAddress" : "mother@nature.co.uk",
					 "mobilePhone" : "3251231234",
					 "relationship" : "parent",
					 "accessConsent" : true
				 }
requestBody.relatedContacts = [
			relatedcontact,
			relatedcontact1
		]
const result = async () => {
	await graphServiceClient.education.usersById("educationUser-id").patch(requestBody);
}


```