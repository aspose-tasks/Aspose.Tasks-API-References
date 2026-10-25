---
title: "Enum ApplicationInfo"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Aspose.Tasks.ApplicationInfo enum. Specificeert de projectversie waarin het bestand is gemaakt"
type: docs
weight: 10
url: /nl/net/aspose.tasks/applicationinfo/
---
## ApplicationInfo enumeration

Specificeert de projectversie waarin het bestand is gemaakt.

```csharp
public enum ApplicationInfo
```

### Waarden

| Naam | Waarde | Beschrijving |
| --- | --- | --- |
| Undefined | `0` | Kan niet worden gedefinieerd. |
| MSP2000 | `1` | Bestand is gemaakt in Microsoft Project 2000/2002. |
| MSP2003 | `2` | Bestand is gemaakt in Microsoft Project 2003. |
| MSP2007 | `3` | Bestand is gemaakt in Microsoft Project 2007. |
| MSP2010 | `4` | Bestand is gemaakt in Microsoft Project 2010. |
| MSP2013 | `5` | Bestand is gemaakt in Microsoft Project 2013. |
| MSP2016 | `6` | Bestand is gemaakt in Microsoft Project 2016. |

## Voorbeelden

Toont hoe projecttoepassingsinformatie kan worden gecontroleerd.

```csharp
var info = Project.GetProjectFileInfo(DataDir + "Project.xml");
Console.WriteLine("CanRead: " + info.CanRead);
Console.WriteLine("ProjectApplicationInfo: " + info.ProjectApplicationInfo);
Console.WriteLine("ProjectFileFormat: " + info.ProjectFileFormat);
```

### Zie ook

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


