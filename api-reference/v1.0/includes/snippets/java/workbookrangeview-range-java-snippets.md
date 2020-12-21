---
description: "Automatically generated file. DO NOT MODIFY"
---

```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookRange workbookRange = graphClient.me().drive().root().workbook().worksheets("{id}")
	.range(WorkbookRangeRangeParameterSet
		.newBuilder()
		.withAddress("A1:Z10")
		.build())
	.visibleView()
	.range()
	.buildRequest()
	.get();

```