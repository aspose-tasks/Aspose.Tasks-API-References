---
title: "ProjectServerManager.GetProjectList"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Metode ProjectServerManager. Mengambil daftar proyek dari Working store akun Project Online saat ini dan instance Project Server."
type: docs
weight: 50
url: /id/net/aspose.tasks/projectservermanager/getprojectlist/
---
## ProjectServerManager.GetProjectList method

Mengambil daftar proyek dari penyimpanan 'Working' akun Project Online saat ini \\ instance Project Server.

```csharp
public IEnumerable<ProjectInfo> GetProjectList()
```

### Nilai Kembali

Enumerasi proyek dalam akun Project Online saat ini \ instance Project Server.

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

* class [ProjectInfo](../../projectinfo/)
* class [ProjectServerManager](../)
* namespace [Aspose.Tasks](../../projectservermanager/)
* assembly [Aspose.Tasks](../../../)


