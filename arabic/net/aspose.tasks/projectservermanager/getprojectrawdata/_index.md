---
title: ProjectServerManager.GetProjectRawData
second_title: Aspose.Tasks لمرجع .NET API
description: ProjectServerManager طريقة. يحصل على البيانات الثنائية للمشروع لأغراض استكشاف الأخطاء وإصلاحها.
type: docs
weight: 60
url: /ar/net/aspose.tasks/projectservermanager/getprojectrawdata/
---
## ProjectServerManager.GetProjectRawData method

يحصل على البيانات الثنائية للمشروع لأغراض استكشاف الأخطاء وإصلاحها.

```csharp
public Stream GetProjectRawData(Guid projectGuid)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| projectGuid | Guid | دليل مشروع القراءة. |

### قيمة الإرجاع

دفق يحتوي على بيانات المشروع الأولية.

### أمثلة

```csharp
In this example the debug info for the specific project is retrieved. You can pass the resulting "debug.zip" to the support team for troubleshooting purposes.
[C#]
var credentials = new ProjectServerCredentials("https://xxxxxx.sharepoint.com "،" yyyyy@xxxxxxx.onmicrosoft.com "،" password ") ;
// دليل المشروع الذي تحاول الحصول عليه.
var projectGuid = new Guid("e0294bfb-5657-45c8-9cc5-82169fb95d69");
ProjectServerManager manager = new ProjectServerManager(credentials);
using (var fileStream = File.OpenWrite(@"c:\debug.zip"))
{
    using (var stream = manager.GetProjectRawData(projectGuid))
    {
        stream.CopyTo(fileStream);
    }
}
```

### أنظر أيضا

* class [ProjectServerManager](../)
* مساحة الاسم [Aspose.Tasks](../../projectservermanager/)
* المجسم [Aspose.Tasks](../../../)


