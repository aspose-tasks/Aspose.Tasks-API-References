---
title: "ProjectServerSaveOptions.ProjectName"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Properti ProjectServerSaveOptions. Mendapatkan atau mengatur nama proyek yang ditampilkan dalam daftar proyek Project Server Project Online. Harus unik dalam instance Project Server Project Online. Jika nilai dihilangkan, nilai properti Prj.Name akan digunakan sebagai gantinya."
type: docs
weight: 40
url: /id/net/aspose.tasks/projectserversaveoptions/projectname/
---
## ProjectServerSaveOptions.ProjectName property

Mendapatkan atau mengatur nama proyek yang ditampilkan dalam daftar proyek Project Server \ Project Online. Harus unik dalam instance Project Server \ Project Online. Jika nilai dihilangkan, nilai properti Prj.Name akan digunakan sebagai gantinya.

```csharp
public string ProjectName { get; set; }
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


