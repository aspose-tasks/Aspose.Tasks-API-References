---
title: "ProjectServerManager.GetProjectRawData"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Metode ProjectServerManager. Mengambil data biner proyek untuk tujuan pemecahan masalah."
type: docs
weight: 60
url: /id/net/aspose.tasks/projectservermanager/getprojectrawdata/
---
## ProjectServerManager.GetProjectRawData method

Mengambil data biner proyek untuk keperluan pemecahan masalah.

```csharp
public Stream GetProjectRawData(Guid projectGuid)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| projectGuid | Guid | Guid proyek yang akan dibaca. |

### Nilai Kembali

Stream yang berisi data mentah proyek.

## Contoh

```csharp
In this example the debug info for the specific project is retrieved. You can pass the resulting "debug.zip" to the support team for troubleshooting purposes.
[C#]
var credentials = new ProjectServerCredentials("https://xxxxxx.sharepoint.com", "yyyyy@xxxxxxx.onmicrosoft.com", "password");
// GUID dari proyek yang ingin Anda dapatkan.
var projectGuid = new Guid("e0294bfb-5657-45c8-9cc5-82169fb95d69");
ProjectServerManager manager = new ProjectServerManager(credentials);
using (var fileStream = File.OpenWrite(@"c:\debug.zip"))
{
    using (var stream = manager.GetProjectRawData(projectGuid))
    {
        stream.CopyTo(fileStream);
    }
}
```

Menampilkan cara mengambil data mentah proyek dari Microsoft Project Online untuk tujuan pemecahan masalah.

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

    // Pengguna dapat membaca proyek sebagai stream data mentah untuk tujuan pemecahan masalah.
    using (FileStream fs = File.Create(OutDir + "projectRawData.zip"))
    {
        using (var stream = manager.GetProjectRawData(info.Id))
        {
            stream.CopyTo(fs);
        }
    }

    // Anda dapat mengirimkan file hasil tersebut ke tim dukungan.
}
```

### Lihat Juga

* class [ProjectServerManager](../)
* namespace [Aspose.Tasks](../../projectservermanager/)
* assembly [Aspose.Tasks](../../../)


