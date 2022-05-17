---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new ConditionalAccessPolicy();
requestBody.displayName = "Demo app for documentation";
requestBody.state = ConditionalAccessPolicyState.Disabled;
requestBody.conditions = new ConditionalAccessConditionSet();
requestBody.conditions.signInRiskLevels = [
				"high",
				"medium"
			]
requestBody.conditions.clientAppTypes = [
				"mobileAppsAndDesktopClients",
				"exchangeActiveSync",
				"other"
			]
requestBody.conditions.applications = new ConditionalAccessApplications();
requestBody.conditions.applications.includeApplications = [
					"All"
				]
requestBody.conditions.applications.excludeApplications = [
					"499b84ac-1321-427f-aa17-267ca6975798",
					"00000007-0000-0000-c000-000000000000",
					"de8bc8b5-d9f9-48b1-a8ad-b748da725064",
					"00000012-0000-0000-c000-000000000000",
					"797f4846-ba00-4fd7-ba43-dac1f8f63013",
					"05a65629-4c1b-48c1-a78b-804c4abdd4af",
					"7df0a125-d3be-4c96-aa54-591f83ff541c"
				]
requestBody.conditions.applications.includeUserActions = [
				]
requestBody.conditions.users = new ConditionalAccessUsers();
requestBody.conditions.users.includeUsers = [
					"a702a13d-a437-4a07-8a7e-8c052de62dfd"
				]
requestBody.conditions.users.excludeUsers = [
					"124c5b6a-ffa5-483a-9b88-04c3fce5574a",
					"GuestsOrExternalUsers"
				]
requestBody.conditions.users.includeGroups = [
				]
requestBody.conditions.users.excludeGroups = [
				]
requestBody.conditions.users.includeRoles = [
					"9b895d92-2cd3-44c7-9d02-a6ac2d5ea5c3",
					"cf1c38e5-3621-4004-a7cb-879624dced7c",
					"c4e39bd9-1100-46d3-8c65-fb160da0071f"
				]
requestBody.conditions.users.excludeRoles = [
					"b0f54661-2d74-4c50-afa3-1ec803f12efe"
				]
requestBody.conditions.platforms = new ConditionalAccessPlatforms();
requestBody.conditions.platforms.includePlatforms = [
					"all"
				]
requestBody.conditions.platforms.excludePlatforms = [
					"iOS",
					"windowsPhone"
				]
requestBody.conditions.locations = new ConditionalAccessLocations();
requestBody.conditions.locations.includeLocations = [
					"AllTrusted"
				]
requestBody.conditions.locations.excludeLocations = [
					"00000000-0000-0000-0000-000000000000",
					"d2136c9c-b049-47ae-b9cf-316e04ef7198"
				]
requestBody.grantControls = new ConditionalAccessGrantControls();
requestBody.grantControls.operator = "OR";
requestBody.grantControls.builtInControls = [
				"mfa",
				"compliantDevice",
				"domainJoinedDevice",
				"approvedApplication",
				"compliantApplication"
			]
requestBody.grantControls.customAuthenticationFactors = [
			]
requestBody.grantControls.termsOfUse = [
				"ce580154-086a-40fd-91df-8a60abac81a0",
				"7f29d675-caff-43e1-8a53-1b8516ed2075"
			]
requestBody.sessionControls = new ConditionalAccessSessionControls();
requestBody.sessionControls.applicationEnforcedRestrictions = null,
requestBody.sessionControls.persistentBrowser = null,
requestBody.sessionControls.cloudAppSecurity = new CloudAppSecuritySessionControl();
requestBody.sessionControls.cloudAppSecurity.cloudAppSecurityType = CloudAppSecuritySessionControlType.BlockDownloads;
requestBody.sessionControls.cloudAppSecurity.isEnabled = true;
requestBody.sessionControls.signInFrequency = new SignInFrequencySessionControl();
requestBody.sessionControls.signInFrequency.value = 4;
requestBody.sessionControls.signInFrequency.type = SigninFrequencyType.Hours;
requestBody.sessionControls.signInFrequency.isEnabled = true;
const result = async () => {
	await graphServiceClient.identity.conditionalAccess.policies.post(requestBody);
}


```