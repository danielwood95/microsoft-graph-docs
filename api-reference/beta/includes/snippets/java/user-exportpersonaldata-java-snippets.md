---
description: "Automatically generated file. DO NOT MODIFY"
---

```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String storageLocation = "storageLocation-value";

graphClient.users("{id}")
	.exportPersonalData(UserExportPersonalDataParameterSet
		.newBuilder()
		.withStorageLocation(storageLocation)
		.build())
	.buildRequest()
	.post();

```