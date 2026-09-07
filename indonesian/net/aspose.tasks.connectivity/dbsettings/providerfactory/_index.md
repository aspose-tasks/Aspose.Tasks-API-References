---
title: "DbSettings.ProviderFactory"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Properti DbSettings. Mendapatkan atau mengatur sebuah instance dari DbProviderFactory yang digunakan untuk terhubung ke DB. Jika kedua ProviderFactory dan ProviderInvariantName diatur, ProviderFactory memiliki prioritas. Nilai default adalah null"
type: docs
weight: 30
url: /id/net/aspose.tasks.connectivity/dbsettings/providerfactory/
---
## DbSettings.ProviderFactory property

Mendapatkan atau mengatur instance DbProviderFactory yang digunakan untuk terhubung ke DB. Jika kedua ProviderFactory dan ProviderInvariantName diatur, ProviderFactory memiliki prioritas. Nilai default adalah null.

```csharp
public DbProviderFactory ProviderFactory { get; set; }
```

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

### Lihat Juga

* class [DbSettings](../)
* namespace [Aspose.Tasks.Connectivity](../../dbsettings/)
* assembly [Aspose.Tasks](../../../)


