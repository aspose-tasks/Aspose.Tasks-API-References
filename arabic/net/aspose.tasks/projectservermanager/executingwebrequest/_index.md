---
title: "ProjectServerManager.ExecutingWebRequest"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "حدث ProjectServerManager. حدث يُطلق عندما يتم إرسال طلب الويب إلى واجهة برمجة تطبيقات Project Servers."
type: docs
weight: 20
url: /ar/net/aspose.tasks/projectservermanager/executingwebrequest/
---
## ProjectServerManager.ExecutingWebRequest event

حدث يُطلق عندما يتم إرسال طلب الويب إلى واجهة برمجة تطبيقات الويب الخاصة بـ Project Server.

```csharp
public event EventHandler<WebRequestEventArgs> ExecutingWebRequest;
```

## الأمثلة

يوضح كيفية استخدام حدث ProjectServerManager.ExecutingWebRequest لتخصيص طلبات الويب الموجهة إلى Project Server.

```csharp
try
{
    const string SiteUrl = "https://myprojectserver/sites/pwa";
    const string UserName = "test_user";
    const string Password = "MyPassword";

    var credentials = new ProjectServerCredentials(SiteUrl, new NetworkCredential(UserName, Password));

    var project = new Project(DataDir + @"Project1.mpp");

    var manager = new ProjectServerManager(credentials);
    manager.ExecutingWebRequest += delegate (object sender, WebRequestEventArgs e)
    {
        e.WebRequest.Headers.Add("XMyCustomHeader", "testvalue");
    };

    var list = manager.GetProjectList();
}
catch (ProjectOnlineException ex)
{
    Console.WriteLine(ex.Message);
}
```

### انظر أيضًا

* class [WebRequestEventArgs](../../webrequesteventargs/)
* class [ProjectServerManager](../)
* namespace [Aspose.Tasks](../../projectservermanager/)
* assembly [Aspose.Tasks](../../../)


