---
description: "Automatically generated file. DO NOT MODIFY"
---

```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ReportRootGetAzureADApplicationSignInSummaryCollectionPage getAzureADApplicationSignInSummary = graphClient.reports()
	.getAzureADApplicationSignInSummary(ApplicationSignInSummary)GetAzureADApplicationSignInSummaryParameterSet
		.newBuilder()
		.withPeriod("D7")
		.build())
	.buildRequest()
	.get();

```