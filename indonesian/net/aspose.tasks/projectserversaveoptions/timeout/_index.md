---
title: "ProjectServerSaveOptions.Timeout"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Properti ProjectServerSaveOptions. Mendapatkan atau mengatur batas waktu yang digunakan saat menunggu pemrosesan permintaan penyimpanan proyek oleh layanan pemrosesan antrian Project Servers. Nilai default untuk properti ini adalah 1 menit."
type: docs
weight: 50
url: /id/net/aspose.tasks/projectserversaveoptions/timeout/
---
## ProjectServerSaveOptions.Timeout property

Mendapatkan atau mengatur batas waktu yang digunakan saat menunggu pemrosesan permintaan penyimpanan proyek oleh layanan pemrosesan antrean Project Server. Nilai default untuk properti ini adalah 1 menit.

```csharp
public TimeSpan Timeout { get; set; }
```

## Catatan

Waktu pemrosesan mungkin lebih lama untuk proyek besar atau jika instance Project Server terlalu sibuk menanggapi permintaan lain.

## Contoh

Menampilkan cara memperbarui proyek di Microsoft Project Online dan mengontrol nilai batas waktu penyimpanan.

```csharp
const string SharepointDomainAddress = "https://contoso.sharepoint.com/sites/pwa";
const string UserName = "admin@contoso.onmicrosoft.com";
const string Password = "MyPassword";

var credentials = new ProjectServerCredentials(SharepointDomainAddress, UserName, Password);
try
{
    var manager = new ProjectServerManager(credentials);

    ProjectInfo projectInfo = null;
    foreach (var info in manager.GetProjectList())
    {
        if (info.Name == "My project")
        {
            projectInfo = info;
        }
    }

    if (projectInfo == null)
    {
        Console.WriteLine("Project 'My project' not found in working store of Project Online account.");
        return;
    }

    var project = manager.GetProject(projectInfo.Id);
    project.Set(Prj.FinishDate, new DateTime(2020, 03, 01));

    var task = project.RootTask.Children.Add("New task");
    task.Set(Tsk.Start, new DateTime(2020, 02, 26));
    task.Set(Tsk.Duration, project.GetDuration(2, TimeUnitType.Day));

    var options = new ProjectServerSaveOptions { Timeout = TimeSpan.FromMinutes(5) };

    manager.UpdateProject(project, options);
}
catch (ProjectOnlineException ex)
{
    Console.WriteLine("Failed to update the project. Error: " + ex);
}
```

### Lihat Juga

* class [ProjectServerSaveOptions](../)
* namespace [Aspose.Tasks](../../projectserversaveoptions/)
* assembly [Aspose.Tasks](../../../)


