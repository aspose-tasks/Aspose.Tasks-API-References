---
title: "Kelas DbSettings"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Kelas Aspose.Tasks.Connectivity.DbSettings. Memungkinkan menentukan pengaturan untuk membaca dari basis data proyek"
type: docs
weight: 290
url: /id/net/aspose.tasks.connectivity/dbsettings/
---
## DbSettings class

Mengizinkan untuk menentukan pengaturan membaca dari basis data proyek.

```csharp
public abstract class DbSettings
```

## Properti

| Nama | Deskripsi |
| --- | --- |
| [ConnectionString](../../aspose.tasks.connectivity/dbsettings/connectionstring/) { get; set; } | Mendapatkan atau mengatur string koneksi. |
| [ProjectLoadingCallback](../../aspose.tasks.connectivity/dbsettings/projectloadingcallback/) { get; set; } | Mendapatkan atau mengatur callback yang akan dipanggil selama operasi pemuatan proyek. |
| [ProviderFactory](../../aspose.tasks.connectivity/dbsettings/providerfactory/) { get; set; } | Mendapatkan atau mengatur instance DbProviderFactory yang digunakan untuk terhubung ke DB. Jika kedua ProviderFactory dan ProviderInvariantName diatur, ProviderFactory memiliki prioritas. Nilai default adalah null. |
| [ProviderInvariantName](../../aspose.tasks.connectivity/dbsettings/providerinvariantname/) { get; set; } | Mendapatkan atau mengatur nama invarian penyedia yang digunakan untuk mendapatkan instance kelas DbProviderFactory. Nilai default adalah SqlClient. |

## Contoh

Menampilkan cara membaca proyek dari file XML Primavera dengan beberapa proyek menggunakan nama penyedia.

```csharp
var connectionString = "Data Source=" + DataDir + "\\PPMDBSQLite.db";

// Buat Pengaturan DB Primavera menggunakan string koneksi dan ID proyek
var settings = new PrimaveraDbSettings(connectionString, 4502);
settings.ProviderInvariantName = "System.Data.SQLite";

Console.WriteLine("Connection String: " + settings.ConnectionString);
Console.WriteLine("Provider Name: " + settings.ProviderInvariantName);

var project = new Project(settings);
project.Save(OutDir + "SupportForSQLiteDatabase_out.mpp", SaveFileFormat.Mpp);
```

### Lihat Juga

* namespace [Aspose.Tasks.Connectivity](../../aspose.tasks.connectivity/)
* assembly [Aspose.Tasks](../../)


