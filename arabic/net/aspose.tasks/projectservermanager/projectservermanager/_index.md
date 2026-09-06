---
title: "ProjectServerManager.ProjectServerManager"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "منشئ ProjectServerManager. يهيئ مثيلًا جديدًا لفئة ProjectServerManager."
type: docs
weight: 10
url: /ar/net/aspose.tasks/projectservermanager/projectservermanager/
---
## ProjectServerManager constructor

يهيئ مثيلًا جديدًا لفئة [`ProjectServerManager`](../).

```csharp
public ProjectServerManager(ProjectServerCredentials credentials)
```

| معامل | النوع | الوصف |
| --- | --- | --- |
| بيانات الاعتماد | ProjectServerCredentials | بيانات الاعتماد المستخدمة للاتصال بحساب Project Online. |

## الأمثلة

يوضح هذا المثال كيفية إنشاء نسخة من ProjectServerManager للوصول إلى نسخة محلية من Project Server.

```csharp
[C#]
string site = "http://project_server_instance.local/";
var windowsCredentials = new NetworkCredential("Administrator", "my_password", "DOMAIN");
var projectServerCredentials = new ProjectServerCredentials(site, windowsCredentials);
ProjectServerManager manager = new ProjectServerManager(projectServerCredentials);
```

يوضح هذا المثال كيفية إنشاء نسخة من ProjectServerManager للوصول إلى حساب في خدمة Project Online.

```csharp
[C#]
var credentials = new ProjectServerCredentials("https://xxxxxx.sharepoint.com", "yyyyy@xxxxxxx.onmicrosoft.com", "password");
ProjectServerManager manager = new ProjectServerManager(projectServerCredentials);
```

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

* class [ProjectServerCredentials](../../projectservercredentials/)
* class [ProjectServerManager](../)
* namespace [Aspose.Tasks](../../projectservermanager/)
* assembly [Aspose.Tasks](../../../)


