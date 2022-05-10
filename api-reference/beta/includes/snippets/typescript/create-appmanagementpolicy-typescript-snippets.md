---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new AppManagementPolicy();
requestBody.displayName = "Credential management policy";
requestBody.description = "Cred policy sample";
requestBody.isEnabled = true;
requestBody.restrictions = new AppManagementConfiguration();
const passwordcredentialconfiguration = new PasswordCredentialConfiguration();
passwordcredentialconfiguration.additionalData = {
						 "restrictionType" : "passwordAddition",
						 "maxLifetime" : null,
						 "restrictForAppsCreatedAfterDateTime" : "2019-10-19T10:37:00Z"
					 }
const passwordcredentialconfiguration1 = new PasswordCredentialConfiguration();
passwordcredentialconfiguration1.additionalData = {
						 "restrictionType" : "passwordLifetime",
						 "maxLifetime" : "P4DT12H30M5S",
						 "restrictForAppsCreatedAfterDateTime" : "2014-10-19T10:37:00Z"
					 }
const passwordcredentialconfiguration2 = new PasswordCredentialConfiguration();
passwordcredentialconfiguration2.additionalData = {
						 "restrictionType" : "symmetricKeyAddition",
						 "maxLifetime" : null,
						 "restrictForAppsCreatedAfterDateTime" : "2019-10-19T10:37:00Z"
					 }
const passwordcredentialconfiguration3 = new PasswordCredentialConfiguration();
passwordcredentialconfiguration3.additionalData = {
						 "restrictionType" : "symmetricKeyLifetime",
						 "maxLifetime" : "P4D",
						 "restrictForAppsCreatedAfterDateTime" : "2014-10-19T10:37:00Z"
					 }
requestBody.restrictions.passwordCredentials = [
				passwordcredentialconfiguration,
				passwordcredentialconfiguration1,
				passwordcredentialconfiguration2,
				passwordcredentialconfiguration3
			]
const keycredentialconfiguration = new KeyCredentialConfiguration();
keycredentialconfiguration.additionalData = {
						 "restrictionType" : "asymmetricKeyLifetime",
						 "maxLifetime" : "P90D",
						 "restrictForAppsCreatedAfterDateTime" : "2014-10-19T10:37:00Z"
					 }
requestBody.restrictions.keyCredentials = [
				keycredentialconfiguration
			]
const result = async () => {
	await graphServiceClient.policies.appManagementPolicies.post(requestBody);
}


```