---
title: "ProjectServerManager.CreateNewProject"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Metode ProjectServerManager. Membuat proyek baru di instance Project Server atau Project Online menggunakan opsi penyimpanan default."
type: docs
weight: 30
url: /id/net/aspose.tasks/projectservermanager/createnewproject/
---
## CreateNewProject(Project) {#createnewproject}

Membuat proyek baru dalam instance Project Server\Project Online menggunakan opsi penyimpanan default.

```csharp
public void CreateNewProject(Project project)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| proyek | Project | Proyek yang akan disimpan ke instance Project Server\Project Online. |

### Pengecualian

| pengecualian | kondisi |
| --- | --- |
| [ProjectOnlineException](../../projectonlineexception/) | Jika terjadi kesalahan komunikasi atau kesalahan yang dikembalikan oleh server. |

## Contoh

Dalam contoh ini proyek dimuat dari file .mpp dan disimpan ke akun Project Online.

```csharp
[C#]
var credentials = new ProjectServerCredentials("https://xxxxxx.sharepoint.com", "yyyyy@xxxxxxx.onmicrosoft.com", "password");
var project = new Project(@"sample.mpp");
ProjectServerManager manager = new ProjectServerManager(credentials);
manager.CreateNewProject(project);
```

Menunjukkan cara menggunakan ProjectServerManager untuk membuat proyek baru di Microsoft Project Online.

```csharp
try
{
    const string SharepointDomainAddress = "https://contoso.sharepoint.com/sites/pwa";
    const string UserName = "admin@contoso.onmicrosoft.com";
    const string Password = "MyPassword";

    var credentials = new ProjectServerCredentials(SharepointDomainAddress, UserName, Password);

    var project = new Project(DataDir + @"Project1.mpp");

    var manager = new ProjectServerManager(credentials);
    manager.CreateNewProject(project);
}
catch (ProjectOnlineException ex)
{
    Console.WriteLine(ex.Message);
}
```

### Lihat Juga

* class [Project](../../project/)
* class [ProjectServerManager](../)
* namespace [Aspose.Tasks](../../projectservermanager/)
* assembly [Aspose.Tasks](../../../)

---

## CreateNewProject(Project, ProjectServerSaveOptions) {#createnewproject_1}

Membuat proyek baru di instance Project Server\\Project Online menggunakan opsi penyimpanan yang ditentukan.

```csharp
public void CreateNewProject(Project project, ProjectServerSaveOptions saveOptions)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| proyek | Project | Proyek yang akan disimpan ke instance Project Server\Project Online. |
| saveOptions | ProjectServerSaveOptions | Instansi dari kelas [`ProjectServerSaveOptions`](../../projectserversaveoptions/). |

### Pengecualian

| pengecualian | kondisi |
| --- | --- |
| [ProjectOnlineException](../../projectonlineexception/) | Jika terjadi kesalahan komunikasi atau kesalahan yang dikembalikan oleh server. |

## Contoh

Dalam contoh ini proyek dimuat dari file .mpp dan disimpan ke akun Project Online.

```csharp
[C#]
var credentials = new ProjectServerCredentials("https://xxxxxx.sharepoint.com", "yyyyy@xxxxxxx.onmicrosoft.com", "password");
var project = new Project(@"sample.mpp");
ProjectServerManager manager = new ProjectServerManager(credentials);
manager.CreateNewProject(project, new ProjectServerSaveOptions
{
    ProjectName = "My new project"
});
```

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

* class [Project](../../project/)
* class [ProjectServerSaveOptions](../../projectserversaveoptions/)
* class [ProjectServerManager](../)
* namespace [Aspose.Tasks](../../projectservermanager/)
* assembly [Aspose.Tasks](../../../)


