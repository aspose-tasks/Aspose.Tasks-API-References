---
title: "ProjectServerSaveOptions.ProjectGuid"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية ProjectServerSaveOptions. تحصل أو تعيين المعرف الفريد للمشروع. يجب أن يكون فريداً داخل مثيل Project Server  Project Online"
type: docs
weight: 30
url: /ar/net/aspose.tasks/projectserversaveoptions/projectguid/
---
## ProjectServerSaveOptions.ProjectGuid property

يحصل أو يضبط المعرف الفريد للمشروع. يجب أن يكون فريدًا داخل مثيل Project Server \ Project Online.

```csharp
public Guid ProjectGuid { get; set; }
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


