---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new PrinterShare();
requestBody.displayName = "ShareName";
requestBody.allowAllUsers = true;
requestBody.additionalData = {
		 "printer@odata.bind" : "https://graph.microsoft.com/beta/print/printers/{id}"
	 }
const result = async () => {
	await graphServiceClient.print.sharesById("printerShare-id").patch(requestBody);
}


```