---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new TenantAppManagementPolicy();
requestBody.isEnabled = true;
requestBody.applicationRestrictions = new AppManagementConfiguration();
const passwordcredentialconfiguration = new PasswordCredentialConfiguration();
passwordcredentialconfiguration.additionalData = {
						 "restrictionType" : "passwordAddition",
						 "maxLifetime" : null,
						 "restrictForAppsCreatedAfterDateTime" : "2021-01-01T10:37:00Z"
					 }
const passwordcredentialconfiguration1 = new PasswordCredentialConfiguration();
passwordcredentialconfiguration1.additionalData = {
						 "restrictionType" : "passwordLifetime",
						 "maxLifetime" : "P4DT12H30M5S",
						 "restrictForAppsCreatedAfterDateTime" : "2017-01-01T10:37:00Z"
					 }
const passwordcredentialconfiguration2 = new PasswordCredentialConfiguration();
passwordcredentialconfiguration2.additionalData = {
						 "restrictionType" : "symmetricKeyAddition",
						 "maxLifetime" : null,
						 "restrictForAppsCreatedAfterDateTime" : "2021-01-01T10:37:00Z"
					 }
const passwordcredentialconfiguration3 = new PasswordCredentialConfiguration();
passwordcredentialconfiguration3.additionalData = {
						 "restrictionType" : "customPasswordAddition",
						 "maxLifetime" : null,
						 "restrictForAppsCreatedAfterDateTime" : "2015-01-01T10:37:00Z"
					 }
const passwordcredentialconfiguration4 = new PasswordCredentialConfiguration();
passwordcredentialconfiguration4.additionalData = {
						 "restrictionType" : "symmetricKeyLifetime",
						 "maxLifetime" : "P40D",
						 "restrictForAppsCreatedAfterDateTime" : "2015-01-01T10:37:00Z"
					 }
requestBody.applicationRestrictions.passwordCredentials = [
				passwordcredentialconfiguration,
				passwordcredentialconfiguration1,
				passwordcredentialconfiguration2,
				passwordcredentialconfiguration3,
				passwordcredentialconfiguration4
			]
const keycredentialconfiguration = new KeyCredentialConfiguration();
keycredentialconfiguration.additionalData = {
						 "restrictionType" : "asymmetricKeyLifetime",
						 "maxLifetime" : "P30D",
						 "restrictForAppsCreatedAfterDateTime" : "2015-01-01T10:37:00Z"
					 }
requestBody.applicationRestrictions.keyCredentials = [
				keycredentialconfiguration
			]
const result = async () => {
	await graphServiceClient.policies.defaultAppManagementPolicy.patch(requestBody);
}


```