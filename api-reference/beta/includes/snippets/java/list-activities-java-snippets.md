---
description: "Automatically generated file. DO NOT MODIFY"
---

```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ItemActivityOLDCollectionPage activities = graphClient.me().drive().activities()
	.buildRequest()
	.get();

```