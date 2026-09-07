---
title: "MpdSettings.ProjectId"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Properti MpdSettings. Mendapatkan id dari proyek yang akan dibaca"
type: docs
weight: 20
url: /id/net/aspose.tasks.connectivity/mpdsettings/projectid/
---
## MpdSettings.ProjectId property

Mendapatkan ID proyek yang akan dibaca.

```csharp
public int ProjectId { get; }
```

## Contoh

Menampilkan cara menggunakan pengaturan MPD untuk mengendalikan impor proyek dari basis data.

```csharp
var settings = new MpdSettings("Provider=Microsoft.Jet.OLEDB.4.0; Data Source=" + DataDir + "MpdFileToRead.mpd", 1);

Console.WriteLine("Project ID to load: " + settings.ProjectId);

var project = new Project(settings);
Console.WriteLine(project.Get(Prj.Name));
```

### Lihat Juga

* class [MpdSettings](../)
* namespace [Aspose.Tasks.Connectivity](../../mpdsettings/)
* assembly [Aspose.Tasks](../../../)


