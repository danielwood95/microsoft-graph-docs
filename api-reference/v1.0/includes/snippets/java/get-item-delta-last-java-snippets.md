---
description: "Automatically generated file. DO NOT MODIFY"
---

```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DriveItemDeltaCollectionPage delta = graphClient.me().drive().root()
	.delta(DriveItem)DeltaParameterSet
		.newBuilder()
		.withToken("1230919asd190410jlka")
		.build())
	.buildRequest()
	.get();

```