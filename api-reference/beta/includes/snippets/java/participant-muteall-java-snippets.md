---
description: "Automatically generated file. DO NOT MODIFY"
---

```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<String> participantsList = new LinkedList<String>();
participantsList.add("");

String clientContext = "clientContext-value";

graphClient.communications().calls("{id}").participants()
	.muteAll(MuteParticipantsOperationMuteAllParameterSet
		.newBuilder()
		.withParticipants(participantsList)
		.withClientContext(clientContext)
		.build())
	.buildRequest()
	.post();

```