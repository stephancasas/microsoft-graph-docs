---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new Place();
requestBody.displayName = "Building 1";
requestBody.phone = "555-555-0100";
requestBody.address = new PhysicalAddress();
requestBody.address.street = "4567 Main Street";
requestBody.address.city = "Buffalo";
requestBody.address.state = "NY";
requestBody.address.postalCode = "98052";
requestBody.address.countryOrRegion = "USA";
requestBody.geoCoordinates = new OutlookGeoCoordinates();
requestBody.geoCoordinates.altitude = null,
requestBody.geoCoordinates.latitude = 47.0;
requestBody.geoCoordinates.longitude = -122.0;
requestBody.geoCoordinates.accuracy = null,
requestBody.geoCoordinates.altitudeAccuracy = null,
requestBody.additionalData = {
		 "@odata.type" : "microsoft.graph.roomList"
	 }
const result = async () => {
	await graphServiceClient.placesById("place-id").patch(requestBody);
}


```