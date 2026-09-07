---
title: "ProjectServerSaveOptions.ProjectServerSaveOptions"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Konstruktor ProjectServerSaveOptions. Menginisialisasi instance baru dari kelas ProjectServerSaveOptions"
type: docs
weight: 10
url: /id/net/aspose.tasks/projectserversaveoptions/projectserversaveoptions/
---
## ProjectServerSaveOptions constructor

Menginisialisasi instance baru dari kelas [`ProjectServerSaveOptions`](../).

```csharp
public ProjectServerSaveOptions()
```

## Contoh

Menampilkan cara menggunakan opsi &lt;see cref="Aspose.Tasks.ProjectServerSaveOptions" /&gt; untuk membuat proyek baru dalam instance Project Server yang di‑lokasi.

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

### Lihat Juga

* class [ProjectServerSaveOptions](../)
* namespace [Aspose.Tasks](../../projectserversaveoptions/)
* assembly [Aspose.Tasks](../../../)


