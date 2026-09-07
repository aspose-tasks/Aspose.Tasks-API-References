---
title: "Kelas ProjectServerSaveOptions"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Kelas Aspose.Tasks.ProjectServerSaveOptions. Memungkinkan menentukan opsi tambahan saat proyek disimpan ke Project Server atau Project Online"
type: docs
weight: 1510
url: /id/net/aspose.tasks/projectserversaveoptions/
---
## ProjectServerSaveOptions class

Memungkinkan untuk menentukan opsi tambahan ketika proyek disimpan ke Project Server atau Project Online.

```csharp
public sealed class ProjectServerSaveOptions
```

## Konstruktor

| Nama | Deskripsi |
| --- | --- |
| [ProjectServerSaveOptions](projectserversaveoptions/)() | Menginisialisasi instance baru dari kelas `ProjectServerSaveOptions`. |

## Properti

| Nama | Deskripsi |
| --- | --- |
| [PollingInterval](../../aspose.tasks/projectserversaveoptions/pollinginterval/) { get; set; } | Mendapatkan atau mengatur interval antara permintaan status pekerjaan antrean. Nilai default adalah 2 detik. |
| [ProjectGuid](../../aspose.tasks/projectserversaveoptions/projectguid/) { get; set; } | Mendapatkan atau mengatur pengidentifikasi unik dari sebuah proyek. Harus unik dalam instance Project Server \ Project Online. |
| [ProjectName](../../aspose.tasks/projectserversaveoptions/projectname/) { get; set; } | Mendapatkan atau mengatur nama proyek yang ditampilkan dalam daftar proyek Project Server \ Project Online. Harus unik dalam instance Project Server \ Project Online. Jika nilai dihilangkan, nilai properti Prj.Name akan digunakan sebagai gantinya. |
| [Timeout](../../aspose.tasks/projectserversaveoptions/timeout/) { get; set; } | Mendapatkan atau mengatur batas waktu yang digunakan saat menunggu pemrosesan permintaan penyimpanan proyek oleh layanan pemrosesan antrean Project Server. Nilai default untuk properti ini adalah 1 menit. |

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


