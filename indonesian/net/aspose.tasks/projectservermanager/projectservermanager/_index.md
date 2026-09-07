---
title: "ProjectServerManager.ProjectServerManager"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Konstruktor ProjectServerManager. Menginisialisasi sebuah instansi baru dari kelas ProjectServerManager."
type: docs
weight: 10
url: /id/net/aspose.tasks/projectservermanager/projectservermanager/
---
## ProjectServerManager constructor

Menginisialisasi sebuah instansi baru dari kelas [`ProjectServerManager`](../).

```csharp
public ProjectServerManager(ProjectServerCredentials credentials)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| kredensial | ProjectServerCredentials | Kredensial yang digunakan untuk terhubung ke akun Project Online. |

## Contoh

Contoh ini menunjukkan cara membuat instance dari ProjectServerManager untuk mengakses instance on-premise dari Project Server.

```csharp
[C#]
string site = "http://project_server_instance.local/";
var windowsCredentials = new NetworkCredential("Administrator", "my_password", "DOMAIN");
var projectServerCredentials = new ProjectServerCredentials(site, windowsCredentials);
ProjectServerManager manager = new ProjectServerManager(projectServerCredentials);
```

Contoh ini menunjukkan cara membuat instance dari ProjectServerManager untuk mengakses akun dalam layanan Project Online.

```csharp
[C#]
var credentials = new ProjectServerCredentials("https://xxxxxx.sharepoint.com", "yyyyy@xxxxxxx.onmicrosoft.com", "password");
ProjectServerManager manager = new ProjectServerManager(projectServerCredentials);
```

Menampilkan cara membaca proyek dari Microsoft Project Online.

```csharp
const string SharepointDomainAddress = "https://contoso.sharepoint.com/sites/pwa";
const string UserName = "admin@contoso.onmicrosoft.com";
const string Password = "MyPassword";

var credentials = new ProjectServerCredentials(SharepointDomainAddress, UserName, Password);
var manager = new ProjectServerManager(credentials);
IEnumerable<ProjectInfo> list = manager.GetProjectList();

foreach (var info in list)
{
    var project = manager.GetProject(info.Id);
    Console.WriteLine("{0} - {1} - {2}", info.Name, info.CreatedDate, info.LastSavedDate);
    Console.WriteLine("Resources count: {0}", project.Resources.Count);
}
```

### Lihat Juga

* class [ProjectServerCredentials](../../projectservercredentials/)
* class [ProjectServerManager](../)
* namespace [Aspose.Tasks](../../projectservermanager/)
* assembly [Aspose.Tasks](../../../)


