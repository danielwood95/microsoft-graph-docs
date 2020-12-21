---
description: "Automatically generated file. DO NOT MODIFY"
---

```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookRangeFill workbookRangeFill = new WorkbookRangeFill();
workbookRangeFill.color = "#0000FF";

graphClient.me().drive().items("{id}").workbook().worksheets("{sheet-id}")
	.range(WorkbookRangeRangeParameterSet
		.newBuilder()
		.withAddress("$C$1")
		.build()).format().fill()
	.buildRequest()
	.patch(workbookRangeFill);

```