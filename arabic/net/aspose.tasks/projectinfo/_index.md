---
title: "الفئة ProjectInfo"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "الفئة Aspose.Tasks.ProjectInfo. معلومات موجزة عن المشروع المنشور المتاح على Project Online"
type: docs
weight: 1470
url: /ar/net/aspose.tasks/projectinfo/
---
## ProjectInfo class

معلومات مختصرة عن المشروع المنشور المتاح على Project Online.

```csharp
public sealed class ProjectInfo
```

## المنشئات

| الاسم | الوصف |
| --- | --- |
| [ProjectInfo](projectinfo/)() | يُنشئ مثلاً جديداً من الفئة `ProjectInfo`. |

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [CreatedDate](../../aspose.tasks/projectinfo/createddate/) { get; } | يحصل على التاريخ والوقت عندما تم إنشاء المشروع. |
| [Description](../../aspose.tasks/projectinfo/description/) { get; } | يحصل على وصف المشروع. |
| [Id](../../aspose.tasks/projectinfo/id/) { get; } | يحصل على المعرف الفريد للمشروع. |
| [IsCheckedOut](../../aspose.tasks/projectinfo/ischeckedout/) { get; } | يحصل على قيمة تشير إلى ما إذا كان المشروع تم إخراجه. |
| [LastPublishedDate](../../aspose.tasks/projectinfo/lastpublisheddate/) { get; } | يحصل على أحدث تاريخ تم فيه نشر المشروع. |
| [LastSavedDate](../../aspose.tasks/projectinfo/lastsaveddate/) { get; } | يحصل على أحدث تاريخ تم فيه حفظ المشروع. |
| [Name](../../aspose.tasks/projectinfo/name/) { get; } | يحصل على اسم المشروع. |

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


