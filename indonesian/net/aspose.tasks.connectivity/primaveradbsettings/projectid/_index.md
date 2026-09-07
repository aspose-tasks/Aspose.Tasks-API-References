---
title: "PrimaveraDbSettings.ProjectId"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Properti PrimaveraDbSettings. Mendapatkan id proyek yang akan dibaca"
type: docs
weight: 20
url: /id/net/aspose.tasks.connectivity/primaveradbsettings/projectid/
---
## PrimaveraDbSettings.ProjectId property

Mendapatkan ID proyek yang akan dibaca.

```csharp
public int ProjectId { get; }
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

* class [PrimaveraDbSettings](../)
* namespace [Aspose.Tasks.Connectivity](../../primaveradbsettings/)
* assembly [Aspose.Tasks](../../../)


