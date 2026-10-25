---
title: "ProjectServerManager.GetProjectRawData"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "طريقة ProjectServerManager. تحصل على البيانات الثنائية للمشروعات لأغراض استكشاف الأخطاء."
type: docs
weight: 60
url: /ar/net/aspose.tasks/projectservermanager/getprojectrawdata/
---
## ProjectServerManager.GetProjectRawData method

يحصل على البيانات الثنائية للمشروع لأغراض استكشاف الأخطاء وإصلاحها.

```csharp
public Stream GetProjectRawData(Guid projectGuid)
```

| معامل | النوع | الوصف |
| --- | --- | --- |
| projectGuid | Guid | المعرف Guid للمشروع المراد قراءته. |

### قيمة الإرجاع

دفق يحتوي على بيانات المشروع الخام.

## الأمثلة

```csharp
In this example the debug info for the specific project is retrieved. You can pass the resulting "debug.zip" to the support team for troubleshooting purposes.
[C#]
var credentials = new ProjectServerCredentials("https://xxxxxx.sharepoint.com", "yyyyy@xxxxxxx.onmicrosoft.com", "password");
// معرف GUID للمشروع الذي تحاول الحصول عليه.
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

يوضح كيفية استرجاع البيانات الخام للمشروع من Microsoft Project Online لأغراض استكشاف الأخطاء.

```csharp
const string SharepointDomainAddress = "https://contoso.sharepoint.com/sites/pwa";
const string UserName = "admin@contoso.onmicrosoft.com";
const string Password = "MyPassword";

var credentials = new ProjectServerCredentials(SharepointDomainAddress, UserName, Password);
var manager = new ProjectServerManager(credentials);
IEnumerable<ProjectInfo> list = manager.GetProjectList();

foreach (var info in list)
{
    var project = manager.GetProject(info.Id);
    Console.WriteLine("{0} - {1} - {2}", info.Name, info.CreatedDate, info.LastSavedDate);
    Console.WriteLine("Resources count: {0}", project.Resources.Count);

    // يمكن للمستخدم قراءة المشروع كدفق بيانات خام لأغراض استكشاف الأخطاء.
    using (FileStream fs = File.Create(OutDir + "projectRawData.zip"))
    {
        using (var stream = manager.GetProjectRawData(info.Id))
        {
            stream.CopyTo(fs);
        }
    }

    // يمكنك تمرير الملف الناتج إلى فريق الدعم.
}
```

### انظر أيضًا

* class [ProjectServerManager](../)
* namespace [Aspose.Tasks](../../projectservermanager/)
* assembly [Aspose.Tasks](../../../)


