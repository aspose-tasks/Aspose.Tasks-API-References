---
title: "MpdSettings.ProjectId"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "MpdSettings özelliği. Okunacak projenin kimliğini alır."
type: docs
weight: 20
url: /tr/net/aspose.tasks.connectivity/mpdsettings/projectid/
---
## MpdSettings.ProjectId property

Okunacak projenin kimliğini alır.

```csharp
public int ProjectId { get; }
```

## Örnekler

Veritabanından projenin içe aktarımını kontrol etmek için MPD ayarlarının nasıl kullanılacağını gösterir.

```csharp
var settings = new MpdSettings("Provider=Microsoft.Jet.OLEDB.4.0; Data Source=" + DataDir + "MpdFileToRead.mpd", 1);

Console.WriteLine("Project ID to load: " + settings.ProjectId);

var project = new Project(settings);
Console.WriteLine(project.Get(Prj.Name));
```

### Ayrıca Bakınız

* class [MpdSettings](../)
* namespace [Aspose.Tasks.Connectivity](../../mpdsettings/)
* assembly [Aspose.Tasks](../../../)


