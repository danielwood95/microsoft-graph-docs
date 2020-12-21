---
description: "Automatically generated file. DO NOT MODIFY"
---

```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ServicePrincipalDeltaCollectionPage delta = graphClient.servicePrincipals()
	.delta()
	.buildRequest()
	.get();

```