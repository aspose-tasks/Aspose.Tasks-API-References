---
title: "Kelas ProjectServerCredentials"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Kelas Aspose.Tasks.ProjectServerCredentials. Kredensial yang digunakan untuk terhubung ke Project Online atau instance on-premise dari Project Server"
type: docs
weight: 1490
url: /id/net/aspose.tasks/projectservercredentials/
---
## ProjectServerCredentials class

Kredensial yang digunakan untuk terhubung ke Project Online atau instance Project Server on‑premise.

```csharp
public sealed class ProjectServerCredentials
```

## Konstruktor

| Nama | Deskripsi |
| --- | --- |
| [ProjectServerCredentials](projectservercredentials/#constructor)(string, NetworkCredential) | Menginisialisasi sebuah instance baru dari kelas `ProjectServerCredentials` menggunakan URL endpoint Project Web Access dan kredensial jaringan. |
| [ProjectServerCredentials](projectservercredentials/#constructor_1)(string, string) | Menginisialisasi sebuah instance baru dari kelas `ProjectServerCredentials` menggunakan URL situs SharePoint dan token otorisasi SPOIDCRL yang valid untuk situs PWA (Project Web Access) SharePoint. |
| [ProjectServerCredentials](projectservercredentials/#constructor_2)(string, string, string) | Menginisialisasi sebuah instance baru dari kelas `ProjectServerCredentials` menggunakan URL situs SharePoint, nama pengguna, dan kata sandi. |

## Properti

| Nama | Deskripsi |
| --- | --- |
| [AuthToken](../../aspose.tasks/projectservercredentials/authtoken/) { get; } | Mendapatkan token otorisasi untuk instance SharePoint. |
| [SiteUrl](../../aspose.tasks/projectservercredentials/siteurl/) { get; } | Mendapatkan URL PWA di situs SharePoint atau URL Project Server on-premise. Misalnya, https://your_company_name.sharepoint.com/sites/pwa\"; |
| [UserName](../../aspose.tasks/projectservercredentials/username/) { get; } | Mendapatkan nama pengguna untuk situs SharePoint. |

## Metode

| Nama | Deskripsi |
| --- | --- |
| override [ToString](../../aspose.tasks/projectservercredentials/tostring/)() | Mengembalikan representasi string dari instance ini. |

## Contoh

Menampilkan cara menggunakan kredensial project server untuk mengambil daftar proyek dari Microsoft Project Online.

```csharp
try
{
    const string SharepointDomainAddress = "https://contoso.sharepoint.com/sites/pwa";
    const string UserName = "admin@contoso.onmicrosoft.com";
    const string Password = "MyPassword";

    var credentials = new ProjectServerCredentials(SharepointDomainAddress, UserName, Password);

    var newProject = new Project(DataDir + @"Project1.mpp");

    var manager = new ProjectServerManager(credentials);
    manager.CreateNewProject(newProject);

    IEnumerable<ProjectInfo> list = manager.GetProjectList();

    foreach (var info in list)
    {
        var project = manager.GetProject(info.Id);
        Console.WriteLine("{0} - {1} - {2}", info.Name, info.CreatedDate, info.LastSavedDate);
        Console.WriteLine("Resources count: {0}", project.Resources.Count);
    }
}
catch (ProjectOnlineException ex)
{
    Console.WriteLine(ex.Message);
}
```

### Lihat Juga

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


