---
description: "Automatically generated file. DO NOT MODIFY"
---

```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookRangeFont workbookRangeFont = new WorkbookRangeFont();
workbookRangeFont.underline = "Single";
workbookRangeFont.color = "#FFFFFF";
workbookRangeFont.size = 26d;

graphClient.me().drive().items("{id}").workbook().worksheets("{sheet-id}")
	.range(WorkbookRangeRangeParameterSet
		.newBuilder()
		.withAddress("$C$1")
		.build()).format().font()
	.buildRequest()
	.patch(workbookRangeFont);

```