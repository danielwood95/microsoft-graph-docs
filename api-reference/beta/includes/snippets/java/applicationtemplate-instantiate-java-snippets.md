---
description: "Automatically generated file. DO NOT MODIFY"
---

```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String displayName = "My custom name";

graphClient.applicationTemplates("{id}")
	.instantiate(ApplicationServicePrincipalInstantiateParameterSet
		.newBuilder()
		.withDisplayName(displayName)
		.build())
	.buildRequest()
	.post();

```