---
title: "ProjectServerSaveOptions.PollingInterval"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Properti ProjectServerSaveOptions. Mendapatkan atau mengatur interval antara permintaan status pekerjaan antrian. Nilai default adalah 2 detik"
type: docs
weight: 20
url: /id/net/aspose.tasks/projectserversaveoptions/pollinginterval/
---
## ProjectServerSaveOptions.PollingInterval property

Mendapatkan atau mengatur interval antara permintaan status pekerjaan antrean. Nilai default adalah 2 detik.

```csharp
public TimeSpan PollingInterval { get; set; }
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


