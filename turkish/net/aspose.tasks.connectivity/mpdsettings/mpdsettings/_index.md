---
title: "MpdSettings.MpdSettings"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "MpdSettings yapıcı. MpdSettings sınıfının yeni bir örneğini başlatır."
type: docs
weight: 10
url: /tr/net/aspose.tasks.connectivity/mpdsettings/mpdsettings/
---
## MpdSettings constructor

Yeni bir örnek oluşturur [`MpdSettings`](../) sınıfını.

```csharp
public MpdSettings(string connectionString, int projectId)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| connectionString | Dize | belirtilen bağlantı dizesi. |
| projectId | Int32 | okunacak projenin belirtilen kimliği. |

## Örnekler

Bir MPD dosyasından proje nasıl okunacağını gösterir.

```csharp
DbSettings settings = new MpdSettings("Provider=Microsoft.Jet.OLEDB.4.0; Data Source=" + DataDir + "MpdFileToRead.mpd", 1);
var project = new Project(settings);
Console.WriteLine(project.Get(Prj.Name));
```

### Ayrıca Bakınız

* class [MpdSettings](../)
* namespace [Aspose.Tasks.Connectivity](../../mpdsettings/)
* assembly [Aspose.Tasks](../../../)


