---
title: "MpdSettings.MpdSettings"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Konstruktor MpdSettings. Menginisialisasi sebuah instance baru dari kelas MpdSettings"
type: docs
weight: 10
url: /id/net/aspose.tasks.connectivity/mpdsettings/mpdsettings/
---
## MpdSettings constructor

Menginisialisasi sebuah instance baru dari kelas [`MpdSettings`](../).

```csharp
public MpdSettings(string connectionString, int projectId)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| connectionString | String | string koneksi yang ditentukan. |
| projectId | Int32 | id yang ditentukan dari proyek yang akan dibaca. |

## Contoh

Menampilkan cara membaca proyek dari file MPD.

```csharp
DbSettings settings = new MpdSettings("Provider=Microsoft.Jet.OLEDB.4.0; Data Source=" + DataDir + "MpdFileToRead.mpd", 1);
var project = new Project(settings);
Console.WriteLine(project.Get(Prj.Name));
```

### Lihat Juga

* class [MpdSettings](../)
* namespace [Aspose.Tasks.Connectivity](../../mpdsettings/)
* assembly [Aspose.Tasks](../../../)


