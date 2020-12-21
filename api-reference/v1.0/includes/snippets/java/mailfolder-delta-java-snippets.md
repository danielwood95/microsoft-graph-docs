---
description: "Automatically generated file. DO NOT MODIFY"
---

```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

MailFolderDeltaCollectionPage delta = graphClient.me().mailFolders()
	.delta()
	.buildRequest()
	.get();

```