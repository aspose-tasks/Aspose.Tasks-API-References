---
title: "Kelas ProjectOnlineException"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Kelas Aspose.Tasks.ProjectOnlineException. Mewakili pengecualian yang dilempar ketika kesalahan ditemukan selama interaksi dengan instance Project Online atau Project Server."
type: docs
weight: 1480
url: /id/net/aspose.tasks/projectonlineexception/
---
## ProjectOnlineException class

Mewakili pengecualian yang dilemparkan ketika kesalahan ditemukan selama interaksi dengan instance Project Online atau Project Server.

```csharp
public class ProjectOnlineException : TasksException
```

## Contoh

Menunjukkan cara menangkap pengecualian saat membaca proyek dari MS Project Online.

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

### Lihat Juga

* class [TasksException](../tasksexception/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


