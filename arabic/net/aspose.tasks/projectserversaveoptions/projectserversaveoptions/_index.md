---
title: "ProjectServerSaveOptions.ProjectServerSaveOptions"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "منشئ ProjectServerSaveOptions. يهيئ مثيلاً جديداً من الفئة ProjectServerSaveOptions"
type: docs
weight: 10
url: /ar/net/aspose.tasks/projectserversaveoptions/projectserversaveoptions/
---
## ProjectServerSaveOptions constructor

يهيئ مثيلاً جديداً من الفئة [`ProjectServerSaveOptions`](../).

```csharp
public ProjectServerSaveOptions()
```

## الأمثلة

يوضح كيفية استخدام خيارات &lt;see cref="Aspose.Tasks.ProjectServerSaveOptions" /&gt; لإنشاء مشروع جديد في مثيل Project Server المحلي.

```csharp
try
{
    const string URL = "https://project_server.local/sites/pwa";
    const string Domain = "CONTOSO.COM";
    const string UserName = "Administrator";
    const string Password = "MyPassword";

    var project = new Project(DataDir + @"Project1.mpp");

    var windowsCredentials = new NetworkCredential(UserName, Password, Domain);
    var projectServerCredentials = new ProjectServerCredentials(URL, windowsCredentials);
    var manager = new ProjectServerManager(projectServerCredentials);
    var options = new ProjectServerSaveOptions
                      {
                          ProjectGuid = Guid.NewGuid(),
                          ProjectName = "New project",
                          Timeout = TimeSpan.FromMinutes(5),
                          PollingInterval = TimeSpan.FromSeconds(3)
                      };

    manager.CreateNewProject(project, options);
}
catch (ProjectOnlineException ex)
{
    Console.WriteLine(ex.Message);
}
```

### انظر أيضًا

* class [ProjectServerSaveOptions](../)
* namespace [Aspose.Tasks](../../projectserversaveoptions/)
* assembly [Aspose.Tasks](../../../)


