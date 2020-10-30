---
description: "Automatically generated file. DO NOT MODIFY"
---

```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IGroupCollectionPage groups = graphClient.groups()
	.buildRequest()
	.filter("hasMembersWithLicenseErrors+eq+true,")
	.select("id,displayName")
	.get();

```