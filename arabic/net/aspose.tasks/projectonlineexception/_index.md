---
title: "الفئة ProjectOnlineException"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "الفئة Aspose.Tasks.ProjectOnlineException. تمثّل استثناء يُرمى عندما تُكتشف أخطاء أثناء التفاعل مع Project Online أو مثيل Project Server"
type: docs
weight: 1480
url: /ar/net/aspose.tasks/projectonlineexception/
---
## ProjectOnlineException class

يمثل استثناءً يتم إلقاؤه عندما يتم العثور على أخطاء أثناء التفاعل مع مثيل Project Online أو Project Server.

```csharp
public class ProjectOnlineException : TasksException
```

## الأمثلة

يوضح كيفية التقاط الاستثناء أثناء قراءة مشروع من MS Project Online.

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
    manager.CreateNewProject(project);
}
catch (ProjectOnlineException ex)
{
    Console.WriteLine(ex.Message);
}
```

### انظر أيضًا

* class [TasksException](../tasksexception/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


