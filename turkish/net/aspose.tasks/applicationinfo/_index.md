---
title: "Enum ApplicationInfo"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Aspose.Tasks.ApplicationInfo enum. Dosyanın oluşturulduğu proje sürümünü belirtir."
type: docs
weight: 10
url: /tr/net/aspose.tasks/applicationinfo/
---
## ApplicationInfo enumeration

Dosyanın oluşturulduğu proje sürümünü belirtir.

```csharp
public enum ApplicationInfo
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| Undefined | `0` | Tanımlanamaz. |
| MSP2000 | `1` | Dosya Microsoft Project 2000/2002'de oluşturulmuş. |
| MSP2003 | `2` | Dosya Microsoft Project 2003'te oluşturulmuş. |
| MSP2007 | `3` | Dosya Microsoft Project 2007'de oluşturulmuş. |
| MSP2010 | `4` | Dosya Microsoft Project 2010'da oluşturulmuş. |
| MSP2013 | `5` | Dosya Microsoft Project 2013'te oluşturulmuş. |
| MSP2016 | `6` | Dosya Microsoft Project 2016'da oluşturulmuş. |

## Örnekler

Proje uygulama bilgisini nasıl kontrol edeceğinizi gösterir.

```csharp
var info = Project.GetProjectFileInfo(DataDir + "Project.xml");
Console.WriteLine("CanRead: " + info.CanRead);
Console.WriteLine("ProjectApplicationInfo: " + info.ProjectApplicationInfo);
Console.WriteLine("ProjectFileFormat: " + info.ProjectFileFormat);
```

### Ayrıca Bakınız

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


