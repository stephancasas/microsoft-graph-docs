---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new UploadClientCertificateRequestBody();
requestBody.pkcs12Value = "eyJhbGciOiJSU0EtT0FFUCIsImVuYyI6IkEyNTZHQ00ifQ...kDJ04sJShkkgjL9Bm49plA";
requestBody.password = "<password>";
const result = async () => {
	await graphServiceClient.identity.apiConnectorsById("identityApiConnector-id").uploadClientCertificate.post(requestBody);
}


```