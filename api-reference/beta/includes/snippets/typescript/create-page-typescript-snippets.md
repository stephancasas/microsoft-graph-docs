---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new SitePage();
requestBody.name = "Events.aspx";
requestBody.title = "Team Events";
requestBody.publishingState = new PublicationFacet();
requestBody.publishingState.level = "checkedOut";
requestBody.publishingState.versionId = "0.1";
const webpart = new WebPart();
webpart.additionalData = {
					 "type" : "rte",
						 ["innerHTML" , "<p>Here are the team's upcoming events:</p>"],
				 }
const webpart1 = new WebPart();
webpart1.additionalData = {
					 "type" : "d1d91016-032f-456d-98a4-721247c305e8",
						 ["title" , "Events"],
						 ["description" , "Display upcoming events"],
								 ["title" , ""],
								 ["baseUrl" , "https://www.contoso.com/sites/Engineering"],
								 ["layoutComponentId" , "8ac0c53c-e8d0-4e3e-87d0-7449eb0d4027"],
						 ["dataVersion" , "1.0"],
							 ["selectedListId" , "032e08ab-89b0-4d8f-bc10-73094233615c"],
							 ["selectedCategory" , ""],
							 ["dateRangeOption" , 0],
							 ["startDate" , ""],
							 ["endDate" , ""],
							 ["isOnSeeAllPage" , false],
							 ["layoutId" , "FilmStrip"],
							 ["dataProviderId" , "Event"],
							 ["webId" , "0764c419-1ecc-4126-ba32-0c25ae0fffe8"],
							 ["siteId" , "6b4ffc7a-cfc2-4a76-903a-1cc3686dee23"],
				 }
requestBody.webParts = [
			webpart,
			webpart1
		]
const result = async () => {
	await graphServiceClient.sitesById("site-id").pages.post(requestBody);
}


```