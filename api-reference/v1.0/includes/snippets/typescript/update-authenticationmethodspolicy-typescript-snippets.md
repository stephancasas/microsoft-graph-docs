---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new AuthenticationMethodsPolicy();
requestBody.registrationEnforcement = new RegistrationEnforcement();
requestBody.registrationEnforcement.authenticationMethodsRegistrationCampaign = new AuthenticationMethodsRegistrationCampaign();
requestBody.registrationEnforcement.authenticationMethodsRegistrationCampaign.snoozeDurationInDays = 1;
requestBody.registrationEnforcement.authenticationMethodsRegistrationCampaign.state = AdvancedConfigState.Enabled;
requestBody.registrationEnforcement.authenticationMethodsRegistrationCampaign.excludeTargets = [
				]
const authenticationmethodsregistrationcampaignincludetarget = new AuthenticationMethodsRegistrationCampaignIncludeTarget();
authenticationmethodsregistrationcampaignincludetarget.additionalData = {
							 "id" : "3ee3a9de-0a86-4e12-a287-9769accf1ba2",
							 "targetType" : "group",
							 "targetedAuthenticationMethod" : "microsoftAuthenticator"
						 }
requestBody.registrationEnforcement.authenticationMethodsRegistrationCampaign.includeTargets = [
					authenticationmethodsregistrationcampaignincludetarget
				]
const authenticationmethodconfiguration = new AuthenticationMethodConfiguration();
authenticationmethodconfiguration.additionalData = {
					 "@odata.type" : "#microsoft.graph.fido2AuthenticationMethodConfiguration",
					 "id" : "Fido2",
					 "state" : "disabled",
					 "isSelfServiceRegistrationAllowed" : false,
					 "isAttestationEnforced" : false,
						 ["isEnforced" , false],
						 ["enforcementType" , "block"],
						 ["aaGuids" , [
							]
				 }
requestBody.authenticationMethodConfigurations = [
			authenticationmethodconfiguration
		]
requestBody.additionalData = {
		 "@odata.context" : "https://graph.microsoft.com/v1.0/$metadata#authenticationMethodsPolicy"
	 }
const result = async () => {
	await graphServiceClient.policies.authenticationMethodsPolicy.patch(requestBody);
}


```