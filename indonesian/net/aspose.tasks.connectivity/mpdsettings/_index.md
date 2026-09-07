---
title: "Kelas MpdSettings"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Kelas Aspose.Tasks.Connectivity.MpdSettings. Memungkinkan mengatur opsi yang diperlukan untuk membaca data proyek dari format MPD file basis data MS Access"
type: docs
weight: 300
url: /id/net/aspose.tasks.connectivity/mpdsettings/
---
## MpdSettings class

Mengizinkan untuk mengatur opsi yang diperlukan untuk membaca data proyek dari format MPD (format file basis data MS Access).

```csharp
public class MpdSettings : DbSettings
```

## Konstruktor

| Nama | Deskripsi |
| --- | --- |
| [MpdSettings](mpdsettings/)(string, int) | Menginisialisasi instance baru dari kelas `MpdSettings`. |

## Properti

| Nama | Deskripsi |
| --- | --- |
| [ConnectionString](../../aspose.tasks.connectivity/dbsettings/connectionstring/) { get; set; } | Mendapatkan atau mengatur string koneksi. |
| [ProjectId](../../aspose.tasks.connectivity/mpdsettings/projectid/) { get; } | Mendapatkan ID proyek yang akan dibaca. |
| [ProjectLoadingCallback](../../aspose.tasks.connectivity/dbsettings/projectloadingcallback/) { get; set; } | Mendapatkan atau mengatur callback yang akan dipanggil selama operasi pemuatan proyek. |
| [ProviderFactory](../../aspose.tasks.connectivity/dbsettings/providerfactory/) { get; set; } | Mendapatkan atau mengatur instance DbProviderFactory yang digunakan untuk terhubung ke DB. Jika kedua ProviderFactory dan ProviderInvariantName diatur, ProviderFactory memiliki prioritas. Nilai default adalah null. |
| [ProviderInvariantName](../../aspose.tasks.connectivity/dbsettings/providerinvariantname/) { get; set; } | Mendapatkan atau mengatur nama invarian penyedia yang digunakan untuk mendapatkan instance kelas DbProviderFactory. Nilai default adalah SqlClient. |

## Contoh

Menampilkan cara menggunakan pengaturan MPD untuk mengendalikan impor proyek dari basis data.

```csharp
var settings = new MpdSettings("Provider=Microsoft.Jet.OLEDB.4.0; Data Source=" + DataDir + "MpdFileToRead.mpd", 1);

Console.WriteLine("Project ID to load: " + settings.ProjectId);

var project = new Project(settings);
Console.WriteLine(project.Get(Prj.Name));
```

### Lihat Juga

* class [DbSettings](../dbsettings/)
* namespace [Aspose.Tasks.Connectivity](../../aspose.tasks.connectivity/)
* assembly [Aspose.Tasks](../../)


