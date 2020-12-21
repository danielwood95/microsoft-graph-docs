---
description: "Automatically generated file. DO NOT MODIFY"
---

```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.users("{id | userPrincipalName}").authentication().passwordMethods("{id}")
	.resetPassword(PasswordResetResponseResetPasswordParameterSet
		.newBuilder()
		.withNewPassword(null)
		.withRequireChangeOnNextSignIn(null)
		.build())
	.buildRequest()
	.post();

```