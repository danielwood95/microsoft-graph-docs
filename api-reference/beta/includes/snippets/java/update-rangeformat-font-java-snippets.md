---
description: "Automatically generated file. DO NOT MODIFY"
---

```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookRangeFont workbookRangeFont = new WorkbookRangeFont();
workbookRangeFont.bold = true;
workbookRangeFont.color = "#4B180E";
workbookRangeFont.size = 26d;

graphClient.me().drive().items("{id}").workbook().worksheets("Sheet1")
	.range(WorkbookRangeRangeParameterSet
		.newBuilder()
		.withAddress("$A$1")
		.build()).format().font()
	.buildRequest()
	.patch(workbookRangeFont);

```