---
description: "Automatically generated file. DO NOT MODIFY"
---

```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

KeyCredential keyCredential = new KeyCredential();
keyCredential.type = "X509CertAndPassword";
keyCredential.usage = "Sign";
keyCredential.key = Base64.getDecoder().decode("MIIDYDCCAki...");

PasswordCredential passwordCredential = new PasswordCredential();
passwordCredential.secretText = "MKTr0w1...";

String proof = "eyJ0eXAiOiJ...";

graphClient.applications("{id}")
	.addKey(KeyCredentialAddKeyParameterSet
		.newBuilder()
		.withKeyCredential(keyCredential)
		.withPasswordCredential(passwordCredential)
		.withProof(proof)
		.build())
	.buildRequest()
	.post();

```