---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new BookingService();
requestBody.defaultDuration = "PT1H30M";
requestBody.defaultLocation = new Location();
requestBody.defaultLocation.address = new PhysicalAddress();
requestBody.defaultLocation.address.city = "Buffalo";
requestBody.defaultLocation.address.countryOrRegion = "USA";
requestBody.defaultLocation.address.postalCode = "98052";
requestBody.defaultLocation.address.postOfficeBox = null,
requestBody.defaultLocation.address.state = "NY";
requestBody.defaultLocation.address.street = "4567 First Street";
requestBody.defaultLocation.address.type = null,
requestBody.defaultLocation.address.additionalData = {
				 "@odata.type" : "#microsoft.graph.physicalAddress",
				 "type@odata.type" : "#microsoft.graph.physicalAddressType"
			 }
requestBody.defaultLocation.coordinates = null,
requestBody.defaultLocation.displayName = "Contoso Lunch Delivery";
requestBody.defaultLocation.locationEmailAddress = null,
requestBody.defaultLocation.locationType = null,
requestBody.defaultLocation.locationUri = null,
requestBody.defaultLocation.uniqueId = null,
requestBody.defaultLocation.uniqueIdType = null,
requestBody.defaultLocation.additionalData = {
			 "@odata.type" : "#microsoft.graph.location",
			 "locationType@odata.type" : "#microsoft.graph.locationType",
			 "uniqueIdType@odata.type" : "#microsoft.graph.locationUniqueIdType"
		 }
requestBody.defaultPrice = 10.0;
requestBody.defaultPriceType = BookingPriceType.FixedPrice;
const bookingreminder = new BookingReminder();
bookingreminder.additionalData = {
					 "@odata.type" : "#microsoft.graph.bookingReminder",
					 "message" : "Please be reminded that this service is tomorrow.",
					 "offset" : "P1D",
					 "recipients@odata.type" : "#microsoft.graph.bookingReminderRecipients",
					 "recipients" : "allAttendees"
				 }
requestBody.defaultReminders = [
			bookingreminder
		]
requestBody.description = "Individual bento box lunch delivery";
requestBody.displayName = "Bento";
requestBody.isLocationOnline = true;
requestBody.smsNotificationsEnabled = true;
requestBody.isHiddenFromCustomers = false;
requestBody.notes = "Home-cooked special";
requestBody.postBuffer = "PT10M";
requestBody.preBuffer = "PT5M";
requestBody.schedulingPolicy = new BookingSchedulingPolicy();
requestBody.schedulingPolicy.allowStaffSelection = true;
requestBody.schedulingPolicy.maximumAdvance = "P10D";
requestBody.schedulingPolicy.minimumLeadTime = "PT10H";
requestBody.schedulingPolicy.sendConfirmationsToOwner = true;
requestBody.schedulingPolicy.timeSlotInterval = "PT1H";
requestBody.schedulingPolicy.additionalData = {
			 "@odata.type" : "#microsoft.graph.bookingSchedulingPolicy"
		 }
requestBody.staffMemberIds = [
			"d90d1e8c-5cfe-48cf-a2d5-966267375b6a",
			"2f5f8794-0b29-45b5-b56a-2eb5ff7aa880"
		]
requestBody.additionalData = {
		 "@odata.type" : "#microsoft.graph.bookingService",
		 "defaultPriceType@odata.type" : "#microsoft.graph.bookingPriceType",
		 "defaultReminders@odata.type" : "#Collection(microsoft.graph.bookingReminder)",
		 "staffMemberIds@odata.type" : "#Collection(String)"
	 }
const result = async () => {
	await graphServiceClient.bookingBusinessesById("bookingBusiness-id").services.post(requestBody);
}


```