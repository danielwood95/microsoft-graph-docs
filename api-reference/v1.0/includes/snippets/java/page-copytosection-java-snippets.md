---
description: "Automatically generated file. DO NOT MODIFY"
---

```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String id = "id-value";

String groupId = "groupId-value";

graphClient.me().onenote().pages("{id}")
	.copyToSection(OnenoteOperationCopyToSectionParameterSet
		.newBuilder()
		.withId(id)
		.withGroupId(groupId)
		.withSiteCollectionId(null)
		.withSiteId(null)
		.build())
	.buildRequest()
	.post();

```