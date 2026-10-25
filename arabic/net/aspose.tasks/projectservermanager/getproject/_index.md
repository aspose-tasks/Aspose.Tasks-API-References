---
title: "ProjectServerManager.GetProject"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "طريقة ProjectServerManager. تُعيد المشروع بالمعرف guid المحدد من حساب Project Online ومثيل Project Server."
type: docs
weight: 40
url: /ar/net/aspose.tasks/projectservermanager/getproject/
---
## ProjectServerManager.GetProject method

يحصل على المشروع بالمعرف الفريد المحدد من حساب Project Online \ نسخة Project Server.

```csharp
public Project GetProject(Guid projectGuid)
```

| معامل | النوع | الوصف |
| --- | --- | --- |
| projectGuid | Guid | المعرف Guid للمشروع المراد قراءته. |

### قيمة الإرجاع

مثيل من فئة [`Project`](../../project/) التي تمثل مشروعًا تم قراءته من Project Online \\ Project Server.

## الأمثلة

يظهر كيفية قراءة مشروع من Microsoft Project Online.

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
}
```

### انظر أيضًا

* class [Project](../../project/)
* class [ProjectServerManager](../)
* namespace [Aspose.Tasks](../../projectservermanager/)
* assembly [Aspose.Tasks](../../../)


