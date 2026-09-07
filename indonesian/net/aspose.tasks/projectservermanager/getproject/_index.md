---
title: "ProjectServerManager.GetProject"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Metode ProjectServerManager. Mendapatkan proyek dengan guid yang ditentukan dari akun Project Online instance Project Server"
type: docs
weight: 40
url: /id/net/aspose.tasks/projectservermanager/getproject/
---
## ProjectServerManager.GetProject method

Mengambil proyek dengan guid yang ditentukan dari akun Project Online \\ instance Project Server.

```csharp
public Project GetProject(Guid projectGuid)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| projectGuid | Guid | Guid proyek yang akan dibaca. |

### Nilai Kembali

Instansi kelas [`Project`](../../project/) yang mewakili proyek yang dibaca dari Project Online \ Project Server.

## Contoh

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

* class [Project](../../project/)
* class [ProjectServerManager](../)
* namespace [Aspose.Tasks](../../projectservermanager/)
* assembly [Aspose.Tasks](../../../)


