---
description: "Automatically generated file. DO NOT MODIFY"
---

```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Boolean isSyncedFromOnPremises = false;

graphClient.directoryObjects()
	.getAvailableExtensionProperties(ExtensionProperty)GetAvailableExtensionPropertiesParameterSet
		.newBuilder()
		.withIsSyncedFromOnPremises(isSyncedFromOnPremises)
		.build())
	.buildRequest()
	.post();

```