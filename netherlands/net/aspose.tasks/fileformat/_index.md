---
title: "Enum FileFormat"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Aspose.Tasks.FileFormat enum. Specificeert het bestandsformaat van het project"
type: docs
weight: 590
url: /nl/net/aspose.tasks/fileformat/
---
## FileFormat enumeration

Specificeert het bestandsformaat van het project.

```csharp
public enum FileFormat
```

### Waarden

| Naam | Waarde | Beschrijving |
| --- | --- | --- |
| Undefined | `0` | Kan niet worden gedefinieerd. |
| P6XML | `1` | Stelt het Primavera P6 XML-formaat voor. |
| XML | `2` | Microsoft Project XML-formaat. |
| MPP8 | `3` | Microsoft Project 2000-formaat. |
| MPP9 | `4` | Microsoft Project 2003-formaat. |
| MPP12 | `5` | Microsoft Project 2007-formaat. |
| MPP14 | `6` | Microsoft Project 2010-formaat. |
| MPT9 | `7` | Microsoft Project 2003-sjabloonformaat. |
| MPT12 | `8` | Microsoft Project 2007-sjabloonformaat. |
| MPT14 | `9` | Microsoft Project 2010 (2013) sjabloonindeling. |
| MPX | `10` | Mpx-bestandsindeling |
| XER | `11` | Stelt het Primavera XER-formaat voor. |
| HTML | `12` | Stelt het HTML-formaat voor. |
| ProjectServer | `13` | Project is gelezen van Project Server of Project Online. |

## Voorbeelden

Toont hoe het projectbestandsformaat te lezen.

```csharp
var info = Project.GetProjectFileInfo(DataDir + "Project.xml");
Console.WriteLine("CanRead: " + info.CanRead);
Console.WriteLine("ProjectApplicationInfo: " + info.ProjectApplicationInfo);
Console.WriteLine("ProjectFileFormat: " + info.ProjectFileFormat);
```

### Zie ook

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


