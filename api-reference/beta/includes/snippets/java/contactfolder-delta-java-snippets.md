---
description: "Automatically generated file. DO NOT MODIFY"
---

```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ContactFolderDeltaCollectionPage delta = graphClient.me().contactFolders()
	.delta()
	.buildRequest()
	.get();

```