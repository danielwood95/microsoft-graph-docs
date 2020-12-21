---
description: "Automatically generated file. DO NOT MODIFY"
---

```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookRangeFill workbookRangeFill = new WorkbookRangeFill();
workbookRangeFill.color = "#00FF00";

graphClient.me().drive().items("{id}").workbook().worksheets("Sheet1")
	.range(WorkbookRangeRangeParameterSet
		.newBuilder()
		.withAddress("$B$1")
		.build()).format().fill()
	.buildRequest()
	.patch(workbookRangeFill);

```