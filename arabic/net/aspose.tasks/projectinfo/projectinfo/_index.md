---
title: "ProjectInfo.ProjectInfo"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "منشئ ProjectInfo. ينشئ مثيلاً جديدًا من الفئة ProjectInfo."
type: docs
weight: 10
url: /ar/net/aspose.tasks/projectinfo/projectinfo/
---
## ProjectInfo constructor

ينشئ مثيلاً جديدًا من الفئة [`ProjectInfo`](../).

```csharp
public ProjectInfo()
```

## الأمثلة

يعرض كيفية قراءة المعلومات حول المشاريع من Project Online.

```csharp
const string SharepointDomainAddress = "https://contoso.sharepoint.com/sites/pwa";
const string UserName = "admin@contoso.onmicrosoft.com";
const string Password = "MyPassword";

var credentials = new ProjectServerCredentials(SharepointDomainAddress, UserName, Password);

var reader = new ProjectServerManager(credentials);
IEnumerable<ProjectInfo> list = reader.GetProjectList();

// قراءة معلومات المشروع
Console.WriteLine("Print information about projects:");
foreach (var info in list)
{
    Console.WriteLine("Id: " + info.Id);
    Console.WriteLine("Name: " + info.Name);
    Console.WriteLine("Description: " + info.Description);
    Console.WriteLine("Created Date: " + info.CreatedDate);
    Console.WriteLine("Last Saved Date: " + info.LastSavedDate);
    Console.WriteLine("Last Published Date: " + info.LastPublishedDate);
    Console.WriteLine("Is Checked Out: " + info.IsCheckedOut);
}
```

### انظر أيضًا

* class [ProjectInfo](../)
* namespace [Aspose.Tasks](../../projectinfo/)
* assembly [Aspose.Tasks](../../../)


