---
description: "Automatically generated file. DO NOT MODIFY"
---

```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

UserFindRoomsCollectionPage findRooms = graphClient.me()
	.findRooms(EmailAddress)FindRoomsParameterSet
		.newBuilder()
		.withRoomList("Building2Rooms@contoso.onmicrosoft.com")
		.build())
	.buildRequest()
	.get();

```