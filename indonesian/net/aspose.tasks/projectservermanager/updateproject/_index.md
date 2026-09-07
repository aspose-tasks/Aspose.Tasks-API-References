---
title: "ProjectServerManager.UpdateProject"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Metode ProjectServerManager. Memperbarui proyek yang ada di instance Project ServerProject Online menggunakan opsi penyimpanan default. Proyek yang ada akan ditimpa."
type: docs
weight: 70
url: /id/net/aspose.tasks/projectservermanager/updateproject/
---
## UpdateProject(Project) {#updateproject}

Memperbarui proyek yang ada di instance Project Server\\Project Online menggunakan opsi penyimpanan default. Proyek yang ada akan ditimpa.

```csharp
public void UpdateProject(Project project)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| proyek | Project | Proyek yang akan disimpan ke instance Project Server\Project Online. |

### Pengecualian

| pengecualian | kondisi |
| --- | --- |
| [ProjectOnlineException](../../projectonlineexception/) | Jika terjadi kesalahan komunikasi atau kesalahan yang dikembalikan oleh server. |

## Catatan

Properti 'project.Get(Prj.Guid)' pada Project harus berupa GUID yang valid dari proyek yang ada di akun Project Server \ Project Online.

## Contoh

Dalam contoh ini, proyek dimuat dari akun Project Online, dimodifikasi, dan disimpan kembali ke akun Project Online.

```csharp
[C#]
var credentials = new ProjectServerCredentials("https://xxxxxx.sharepoint.com", "yyyyy@xxxxxxx.onmicrosoft.com", "password");
ProjectServerManager manager = new ProjectServerManager(credentials);
var projectList = manager.GetProjectList();
var projectGuid = projectList.First().Id;
var project = manager.GetProject(projectGuid);
var task = project.RootTask.Children.Add("New task");
manager.UpdateProject(project);
```

Menampilkan cara memperbarui proyek di Microsoft Project Online.

```csharp
const string URL = "https://contoso.sharepoint.com/sites/pwa";
const string Domain = "CONTOSO.COM";
const string UserName = "Administrator";
const string Password = "MyPassword";

var windowsCredentials = new NetworkCredential(UserName, Password, Domain);
var projectServerCredentials = new ProjectServerCredentials(URL, windowsCredentials);
try
{
    var manager = new ProjectServerManager(projectServerCredentials);

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

    manager.UpdateProject(project);
}
catch (ProjectOnlineException ex)
{
    Console.WriteLine("Failed to update the project. Error: " + ex);
}
```

### Lihat Juga

* class [Project](../../project/)
* class [ProjectServerManager](../)
* namespace [Aspose.Tasks](../../projectservermanager/)
* assembly [Aspose.Tasks](../../../)

---

## UpdateProject(Project, ProjectServerSaveOptions) {#updateproject_1}

Memperbarui proyek yang ada di instance Project Server\\Project Online menggunakan opsi penyimpanan yang ditentukan. Proyek yang ada akan ditimpa.

```csharp
public void UpdateProject(Project project, ProjectServerSaveOptions saveOptions)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| proyek | Project | Proyek yang akan disimpan ke instance Project Server\Project Online. |
| saveOptions | ProjectServerSaveOptions | Instansi dari kelas [`ProjectServerSaveOptions`](../../projectserversaveoptions/). |

### Pengecualian

| pengecualian | kondisi |
| --- | --- |
| [ProjectOnlineException](../../projectonlineexception/) | Jika terjadi kesalahan komunikasi atau kesalahan yang dikembalikan oleh server. |

## Catatan

saveOptions.ProjectGuid harus diatur ke GUID dari proyek yang ada pada instance Project Server\ Project Online.

## Contoh

Dalam contoh ini, proyek dimuat dari akun Project Online, dimodifikasi, dan disimpan kembali ke akun Project Online.

```csharp
[C#]
var credentials = new ProjectServerCredentials("https://xxxxxx.sharepoint.com", "yyyyy@xxxxxxx.onmicrosoft.com", "password");
ProjectServerManager manager = new ProjectServerManager(credentials);
var projectList = manager.GetProjectList();
var projectGuid = projectList.First().Id;
var project = manager.GetProject(projectGuid);
var task = project.RootTask.Children.Add("New task");
manager.UpdateProject(project, new ProjectServerSaveOptions
{
    ProjectGuid = projectGuid
});
```

Menampilkan cara memperbarui proyek di Microsoft Project Online dengan penggunaan opsi penyimpanan Project Server.

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

* class [Project](../../project/)
* class [ProjectServerSaveOptions](../../projectserversaveoptions/)
* class [ProjectServerManager](../)
* namespace [Aspose.Tasks](../../projectservermanager/)
* assembly [Aspose.Tasks](../../../)


