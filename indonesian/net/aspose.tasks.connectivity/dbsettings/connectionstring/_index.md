---
title: "DbSettings.ConnectionString"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Properti DbSettings. Mendapatkan atau mengatur string koneksi"
type: docs
weight: 10
url: /id/net/aspose.tasks.connectivity/dbsettings/connectionstring/
---
## DbSettings.ConnectionString property

Mendapatkan atau mengatur string koneksi.

```csharp
public string ConnectionString { get; set; }
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


