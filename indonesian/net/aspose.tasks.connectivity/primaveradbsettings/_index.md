---
title: "Kelas PrimaveraDbSettings"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Kelas Aspose.Tasks.Connectivity.PrimaveraDbSettings. Memungkinkan mengatur opsi yang diperlukan untuk membaca data proyek dari basis data Primavera"
type: docs
weight: 320
url: /id/net/aspose.tasks.connectivity/primaveradbsettings/
---
## PrimaveraDbSettings class

Mengizinkan untuk mengatur opsi yang diperlukan untuk membaca data proyek dari basis data Primavera.

```csharp
public class PrimaveraDbSettings : DbSettings
```

## Konstruktor

| Nama | Deskripsi |
| --- | --- |
| [PrimaveraDbSettings](primaveradbsettings/)(string, int) | Menginisialisasi instance baru dari kelas `PrimaveraDbSettings`. |

## Properti

| Nama | Deskripsi |
| --- | --- |
| [ConnectionString](../../aspose.tasks.connectivity/dbsettings/connectionstring/) { get; set; } | Mendapatkan atau mengatur string koneksi. |
| [ProjectId](../../aspose.tasks.connectivity/primaveradbsettings/projectid/) { get; } | Mendapatkan ID proyek yang akan dibaca. |
| [ProjectLoadingCallback](../../aspose.tasks.connectivity/dbsettings/projectloadingcallback/) { get; set; } | Mendapatkan atau mengatur callback yang akan dipanggil selama operasi pemuatan proyek. |
| [ProviderFactory](../../aspose.tasks.connectivity/dbsettings/providerfactory/) { get; set; } | Mendapatkan atau mengatur instance DbProviderFactory yang digunakan untuk terhubung ke DB. Jika kedua ProviderFactory dan ProviderInvariantName diatur, ProviderFactory memiliki prioritas. Nilai default adalah null. |
| [ProviderInvariantName](../../aspose.tasks.connectivity/dbsettings/providerinvariantname/) { get; set; } | Mendapatkan atau mengatur nama invarian penyedia yang digunakan untuk mendapatkan instance kelas DbProviderFactory. Nilai default adalah SqlClient. |

## Contoh

Menampilkan cara mengimpor proyek dari basis data Primavera.

```csharp
// Inisialisasi instance baru dari kelas PrimaveraDbSettings dengan string koneksi dan ID proyek
var settings = new PrimaveraDbSettings(GetConnectionString(), 4502);
settings.ProviderFactory = SqliteFactory.Instance;

Console.WriteLine("Project UID to read: " + settings.ProjectId);

// baca proyek dengan UID = 4502
var project = new Project(settings);
Console.WriteLine(project.Uid);
Console.WriteLine(project.Name);
Console.WriteLine(project.PrimaveraProperties.ShortName);
```

Menampilkan cara mendapatkan info singkat proyek dari basis data Primavera.

```csharp
var settings = new PrimaveraDbSettings(GetConnectionString(), 0);

var reader = new PrimaveraDbReader(settings);
var projectInfos = reader.GetProjectInfos();

foreach (var info in projectInfos)
{
    Console.WriteLine("{0} - '{1}' - '{2}'", info.Uid, info.ShortName, info.Name);
}

var firstProject = reader.LoadProject(projectInfos[0].Uid);
Console.WriteLine(firstProject.Uid);
Console.WriteLine(firstProject.Name);
Console.WriteLine(firstProject.PrimaveraProperties.ShortName);
```

### Lihat Juga

* class [DbSettings](../dbsettings/)
* namespace [Aspose.Tasks.Connectivity](../../aspose.tasks.connectivity/)
* assembly [Aspose.Tasks](../../)


