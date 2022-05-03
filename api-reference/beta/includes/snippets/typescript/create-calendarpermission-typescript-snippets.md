---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new CalendarPermission();
requestBody.emailAddress = new EmailAddress();
requestBody.emailAddress.name = "Samantha Booth";
requestBody.emailAddress.address = "samanthab@adatum.onmicrosoft.com";
requestBody.isInsideOrganization = true;
requestBody.isRemovable = true;
requestBody.role = CalendarRoleType.Read;
const result = async () => {
	await graphServiceClient.usersById("user-id").calendar.calendarPermissions.post(requestBody);
}


```