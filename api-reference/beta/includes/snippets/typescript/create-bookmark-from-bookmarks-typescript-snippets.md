---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new Bookmark();
requestBody.displayName = "Contoso Install Site";
requestBody.webUrl = "http://www.contoso.com/";
requestBody.description = "Try or buy Contoso for Home or Business and view product information";
requestBody.keywords = new AnswerKeyword();
requestBody.keywords.keywords = [
				"Contoso",
				"install"
			]
requestBody.keywords.reservedKeywords = [
				"Contoso"
			]
requestBody.keywords.matchSimilarKeywords = true;
requestBody.availabilityStartDateTime = null,
requestBody.availabilityEndDateTime = null,
requestBody.platforms = [
			"windows"
		]
const answervariant = new AnswerVariant();
answervariant.additionalData = {
					 "languageTag" : "es-es",
					 "displayName" : "Sitio de instalación Contoso",
					 "description" : "Pruebe o compre Contoso hogar o negocios y vea la información del producto"
				 }
requestBody.targetedVariations = [
			answervariant
		]
requestBody.state = AnswerState.Published;
const result = async () => {
	await graphServiceClient.search.bookmarks.post(requestBody);
}


```