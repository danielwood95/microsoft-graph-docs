---
description: "Automatically generated file. DO NOT MODIFY"
---

```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DirectoryObjectCollectionPage rejectedSenders = graphClient.groups("{id}").rejectedSenders()
	.buildRequest()
	.get();

```