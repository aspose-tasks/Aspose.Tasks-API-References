---
title: "Énumération FileFormat"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Énumération Aspose.Tasks.FileFormat. Spécifie le format de fichier du projet"
type: docs
weight: 590
url: /fr/net/aspose.tasks/fileformat/
---
## FileFormat enumeration

Spécifie le format de fichier du projet.

```csharp
public enum FileFormat
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| Undefined | `0` | Ne peut pas être défini. |
| P6XML | `1` | Représente le format XML Primavera P6. |
| XML | `2` | Format XML Microsoft Project. |
| MPP8 | `3` | Format Microsoft Project 2000. |
| MPP9 | `4` | Format Microsoft Project 2003. |
| MPP12 | `5` | Format Microsoft Project 2007. |
| MPP14 | `6` | Format Microsoft Project 2010. |
| MPT9 | `7` | Format de modèle Microsoft Project 2003. |
| MPT12 | `8` | Format de modèle Microsoft Project 2007. |
| MPT14 | `9` | Format de modèle Microsoft Project 2010 (2013). |
| MPX | `10` | Format de fichier Mpx |
| XER | `11` | Représente le format Primavera XER |
| HTML | `12` | Représente le format HTML |
| ProjectServer | `13` | Le projet a été lu depuis Project Server ou Project Online |

## Exemples

Montre comment lire le format de fichier de vérification de projet.

```csharp
var info = Project.GetProjectFileInfo(DataDir + "Project.xml");
Console.WriteLine("CanRead: " + info.CanRead);
Console.WriteLine("ProjectApplicationInfo: " + info.ProjectApplicationInfo);
Console.WriteLine("ProjectFileFormat: " + info.ProjectFileFormat);
```

### Voir aussi

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


