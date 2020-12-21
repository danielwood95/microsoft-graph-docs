---
description: "Automatically generated file. DO NOT MODIFY"
---

```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Fido2AuthenticationMethodCollectionPage fido2Methods = graphClient.me().authentication().fido2Methods()
	.buildRequest()
	.get();

```