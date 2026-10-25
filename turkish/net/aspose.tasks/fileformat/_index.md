---
title: "Enum FileFormat"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Aspose.Tasks.FileFormat enum. Proje dosya formatını belirtir"
type: docs
weight: 590
url: /tr/net/aspose.tasks/fileformat/
---
## FileFormat enumeration

Projenin dosya biçimini belirtir.

```csharp
public enum FileFormat
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| Undefined | `0` | Tanımlanamaz. |
| P6XML | `1` | Primavera P6 XML formatını temsil eder. |
| XML | `2` | Microsoft Project XML formatı. |
| MPP8 | `3` | Microsoft Project 2000 formatı. |
| MPP9 | `4` | Microsoft Project 2003 formatı. |
| MPP12 | `5` | Microsoft Project 2007 formatı. |
| MPP14 | `6` | Microsoft Project 2010 formatı. |
| MPT9 | `7` | Microsoft Project 2003 şablon formatı. |
| MPT12 | `8` | Microsoft Project 2007 şablon formatı. |
| MPT14 | `9` | Microsoft Project 2010 (2013) şablon biçimi. |
| MPX | `10` | Mpx dosya biçimi |
| XER | `11` | Primavera XER biçimini temsil eder |
| HTML | `12` | HTML biçimini temsil eder |
| ProjectServer | `13` | Proje, Project Server veya Project Online'dan okundu |

## Örnekler

Kontrol proje dosyası biçimini nasıl okuyacağınızı gösterir.

```csharp
var info = Project.GetProjectFileInfo(DataDir + "Project.xml");
Console.WriteLine("CanRead: " + info.CanRead);
Console.WriteLine("ProjectApplicationInfo: " + info.ProjectApplicationInfo);
Console.WriteLine("ProjectFileFormat: " + info.ProjectFileFormat);
```

### Ayrıca Bakınız

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


