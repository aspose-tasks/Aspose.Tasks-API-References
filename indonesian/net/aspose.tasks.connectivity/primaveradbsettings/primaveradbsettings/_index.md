---
title: "PrimaveraDbSettings.PrimaveraDbSettings"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Konstruktor PrimaveraDbSettings. Menginisialisasi sebuah instance baru dari kelas PrimaveraDbSettings"
type: docs
weight: 10
url: /id/net/aspose.tasks.connectivity/primaveradbsettings/primaveradbsettings/
---
## PrimaveraDbSettings constructor

Menginisialisasi sebuah instance baru dari kelas [`PrimaveraDbSettings`](../).

```csharp
public PrimaveraDbSettings(string connectionString, int projectId)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| connectionString | String | string koneksi yang ditentukan. |
| projectId | Int32 | id yang ditentukan dari proyek yang akan dibaca. |

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


