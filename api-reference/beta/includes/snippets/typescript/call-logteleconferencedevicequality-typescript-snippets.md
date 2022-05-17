---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new LogTeleconferenceDeviceQualityRequestBody();
requestBody.quality = new TeleconferenceDeviceQuality();
requestBody.quality.callChainId = "0622673d-9f69-49b3-9d4f-5ec64f42ecce";
requestBody.quality.participantId = "ea078406-b5d4-4d3c-b85e-90103dcec7f6";
requestBody.quality.mediaLegId = "bd9ee398-4b9d-42c7-8b8d-4e8efad9435f";
requestBody.quality.deviceName = "TestAgent";
requestBody.quality.deviceDescription = "TestDescription";
const teleconferencedevicemediaquality = new TeleconferenceDeviceMediaQuality();
teleconferencedevicemediaquality.additionalData = {
						 "@odata.type" : "#microsoft.graph.teleconferenceDeviceAudioQuality",
						 "channelIndex" : 1,
						 "mediaDuration" : "PT20M",
						 "networkLinkSpeedInBytes" : 13000,
						 "localIPAddress" : "127.0.0.1",
						 "localPort" : 6300,
						 "remoteIPAddress" : "102.1.1.101",
						 "remotePort" : 6301,
						 "inboundPackets" : 5500,
						 "outboundPackets" : 5400,
						 "averageInboundPacketLossRateInPercentage" : 0.01,
						 "averageOutboundPacketLossRateInPercentage" : 0.02,
						 "maximumInboundPacketLossRateInPercentage" : 0.05,
						 "maximumOutboundPacketLossRateInPercentage" : 0.06,
						 "averageInboundRoundTripDelay" : "PT0.03S",
						 "averageOutboundRoundTripDelay" : "PT0.04S",
						 "maximumInboundRoundTripDelay" : "PT0.13S",
						 "maximumOutboundRoundTripDelay" : "PT0.14S",
						 "averageInboundJitter" : "PT0.01S",
						 "averageOutboundJitter" : "PT0.015S",
						 "maximumInboundJitter" : "PT0.023S",
						 "maximumOutboundJitter" : "PT0.024S"
					 }
const teleconferencedevicemediaquality1 = new TeleconferenceDeviceMediaQuality();
teleconferencedevicemediaquality1.additionalData = {
						 "@odata.type" : "#microsoft.graph.teleconferenceDeviceVideoQuality",
						 "channelIndex" : 1,
						 "mediaDuration" : "PT20M",
						 "networkLinkSpeedInBytes" : 13000,
						 "localIPAddress" : "127.0.0.1",
						 "localPort" : 6300,
						 "remoteIPAddress" : "102.1.1.101",
						 "remotePort" : 6301,
						 "inboundPackets" : 5500,
						 "outboundPackets" : 5400,
						 "averageInboundPacketLossRateInPercentage" : 0.01,
						 "averageOutboundPacketLossRateInPercentage" : 0.02,
						 "maximumInboundPacketLossRateInPercentage" : 0.05,
						 "maximumOutboundPacketLossRateInPercentage" : 0.06,
						 "averageInboundRoundTripDelay" : "PT0.03S",
						 "averageOutboundRoundTripDelay" : "PT0.04S",
						 "maximumInboundRoundTripDelay" : "PT0.13S",
						 "maximumOutboundRoundTripDelay" : "PT0.14S",
						 "averageInboundJitter" : "PT0.01S",
						 "averageOutboundJitter" : "PT0.015S",
						 "maximumInboundJitter" : "PT0.023S",
						 "maximumOutboundJitter" : "PT0.024S"
					 }
const teleconferencedevicemediaquality2 = new TeleconferenceDeviceMediaQuality();
teleconferencedevicemediaquality2.additionalData = {
						 "@odata.type" : "#microsoft.graph.teleconferenceDeviceScreenSharingQuality",
						 "channelIndex" : 1,
						 "mediaDuration" : "PT20M",
						 "networkLinkSpeedInBytes" : 13000,
						 "localIPAddress" : "127.0.0.1",
						 "localPort" : 6300,
						 "remoteIPAddress" : "102.1.1.101",
						 "remotePort" : 6301,
						 "inboundPackets" : 5500,
						 "outboundPackets" : 5400,
						 "averageInboundPacketLossRateInPercentage" : 0.01,
						 "averageOutboundPacketLossRateInPercentage" : 0.02,
						 "maximumInboundPacketLossRateInPercentage" : 0.05,
						 "maximumOutboundPacketLossRateInPercentage" : 0.06,
						 "averageInboundRoundTripDelay" : "PT0.03S",
						 "averageOutboundRoundTripDelay" : "PT0.04S",
						 "maximumInboundRoundTripDelay" : "PT0.13S",
						 "maximumOutboundRoundTripDelay" : "PT0.14S",
						 "averageInboundJitter" : "PT0.01S",
						 "averageOutboundJitter" : "PT0.015S",
						 "maximumInboundJitter" : "PT0.023S",
						 "maximumOutboundJitter" : "PT0.024S"
					 }
requestBody.quality.mediaQualityList = [
				teleconferencedevicemediaquality,
				teleconferencedevicemediaquality1,
				teleconferencedevicemediaquality2
			]
requestBody.quality.additionalData = {
			 "@odata.type" : "#microsoft.graph.teleconferenceDeviceQuality"
		 }
async () => {
	await graphServiceClient.communications.calls.logTeleconferenceDeviceQuality.post(requestBody);
}


```