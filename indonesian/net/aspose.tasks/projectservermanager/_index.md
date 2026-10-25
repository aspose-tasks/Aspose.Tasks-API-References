---
title: "Kelas ProjectServerManager"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Kelas Aspose.Tasks.ProjectServerManager. Kelas ini menyediakan metode untuk membaca dan melakukan operasi pada proyek dalam akun Project Online yang ditentukan atau dalam instance Project Server on-premise yang ditentukan. Versi Project Server 2016 dan 2019 didukung."
type: docs
weight: 1500
url: /id/net/aspose.tasks/projectservermanager/
---
## ProjectServerManager class

Kelas yang menyediakan metode untuk membaca dan melakukan operasi pada proyek dalam akun Project Online yang ditentukan atau dalam instance Project Server on‑premise yang ditentukan (versi Project Server 2016 dan 2019 didukung).

```csharp
public sealed class ProjectServerManager
```

## Konstruktor

| Nama | Deskripsi |
| --- | --- |
| [ProjectServerManager](projectservermanager/)(ProjectServerCredentials) | Menginisialisasi instance baru dari kelas `ProjectServerManager`. |

## Metode

| Nama | Deskripsi |
| --- | --- |
| [CreateNewProject](../../aspose.tasks/projectservermanager/createnewproject/#createnewproject)(Project) | Membuat proyek baru dalam instance Project Server\Project Online menggunakan opsi penyimpanan default. |
| [CreateNewProject](../../aspose.tasks/projectservermanager/createnewproject/#createnewproject_1)(Project, ProjectServerSaveOptions) | Membuat proyek baru di instance Project Server\\Project Online menggunakan opsi penyimpanan yang ditentukan. |
| [GetProject](../../aspose.tasks/projectservermanager/getproject/)(Guid) | Mengambil proyek dengan guid yang ditentukan dari akun Project Online \\ instance Project Server. |
| [GetProjectList](../../aspose.tasks/projectservermanager/getprojectlist/)() | Mengambil daftar proyek dari penyimpanan 'Working' akun Project Online saat ini \\ instance Project Server. |
| [GetProjectRawData](../../aspose.tasks/projectservermanager/getprojectrawdata/)(Guid) | Mengambil data biner proyek untuk keperluan pemecahan masalah. |
| [UpdateProject](../../aspose.tasks/projectservermanager/updateproject/#updateproject)(Project) | Memperbarui proyek yang ada di instance Project Server\\Project Online menggunakan opsi penyimpanan default. Proyek yang ada akan ditimpa. |
| [UpdateProject](../../aspose.tasks/projectservermanager/updateproject/#updateproject_1)(Project, ProjectServerSaveOptions) | Memperbarui proyek yang ada di instance Project Server\\Project Online menggunakan opsi penyimpanan yang ditentukan. Proyek yang ada akan ditimpa. |

## Peristiwa

| Nama | Deskripsi |
| --- | --- |
| event [ExecutingWebRequest](../../aspose.tasks/projectservermanager/executingwebrequest/) | Sebuah peristiwa yang dipicu ketika permintaan web dikirim ke API web Project Server. |

## Contoh

Menampilkan cara menggunakan manajer Project Server untuk membuat proyek baru dengan opsi penyimpanan yang telah ditentukan pada Microsoft Project Online.

```csharp
try
{
    const string sharepointDomainAddress = "https://contoso.sharepoint.com/sites/pwa";
    const string UserName = "admin@contoso.onmicrosoft.com";
    const string Password = "MyPassword";

    var credentials = new ProjectServerCredentials(sharepointDomainAddress, UserName, Password);

    var project = new Project(DataDir + @"Project1.mpp");

    var manager = new ProjectServerManager(credentials);
    var options = new ProjectServerSaveOptions
    {
        Timeout = TimeSpan.FromSeconds(10)
    };
    manager.CreateNewProject(project, options);
}
catch (ProjectOnlineException ex)
{
    Console.WriteLine(ex.Message);
}
```

### Lihat Juga

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


