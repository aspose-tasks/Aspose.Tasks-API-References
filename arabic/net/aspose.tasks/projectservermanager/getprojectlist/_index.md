---
title: "ProjectServerManager.GetProjectList"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "طريقة ProjectServerManager. تحصل على قائمة المشاريع من المخزن العامل لحساب Project Online الحالي نسخة Project Server."
type: docs
weight: 50
url: /ar/net/aspose.tasks/projectservermanager/getprojectlist/
---
## ProjectServerManager.GetProjectList method

يحصل على قائمة المشاريع من مخزن 'Working' لحساب Project Online الحالي \ نسخة Project Server.

```csharp
public IEnumerable<ProjectInfo> GetProjectList()
```

### قيمة الإرجاع

عدد من المشاريع في حساب Project Online الحالي \ نسخة Project Server.

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

* class [ProjectInfo](../../projectinfo/)
* class [ProjectServerManager](../)
* namespace [Aspose.Tasks](../../projectservermanager/)
* assembly [Aspose.Tasks](../../../)


