---
title: "DbSettings.ProviderInvariantName"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Properti DbSettings. Mendapatkan atau mengatur nama penyedia yang tidak berubah yang digunakan untuk mendapatkan sebuah instance dari kelas DbProviderFactory. Nilai defaultnya adalah SqlClient"
type: docs
weight: 40
url: /id/net/aspose.tasks.connectivity/dbsettings/providerinvariantname/
---
## DbSettings.ProviderInvariantName property

Mendapatkan atau mengatur nama invarian penyedia yang digunakan untuk mendapatkan instance kelas DbProviderFactory. Nilai default adalah SqlClient.

```csharp
public string ProviderInvariantName { get; set; }
```

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

* class [DbSettings](../)
* namespace [Aspose.Tasks.Connectivity](../../dbsettings/)
* assembly [Aspose.Tasks](../../../)


