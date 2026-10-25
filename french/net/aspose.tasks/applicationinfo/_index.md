---
title: "Énumération ApplicationInfo"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Énumération Aspose.Tasks.ApplicationInfo. Spécifie la version du projet dans laquelle le fichier a été créé"
type: docs
weight: 10
url: /fr/net/aspose.tasks/applicationinfo/
---
## ApplicationInfo enumeration

Spécifie la version du projet dans laquelle le fichier a été créé.

```csharp
public enum ApplicationInfo
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| Undefined | `0` | Ne peut pas être défini. |
| MSP2000 | `1` | Le fichier a été créé dans Microsoft Project 2000/2002. |
| MSP2003 | `2` | Le fichier a été créé dans Microsoft Project 2003. |
| MSP2007 | `3` | Le fichier a été créé dans Microsoft Project 2007. |
| MSP2010 | `4` | Le fichier a été créé dans Microsoft Project 2010. |
| MSP2013 | `5` | Le fichier a été créé dans Microsoft Project 2013. |
| MSP2016 | `6` | Le fichier a été créé dans Microsoft Project 2016. |

## Exemples

Montre comment vérifier les informations d'application du projet.

```csharp
var info = Project.GetProjectFileInfo(DataDir + "Project.xml");
Console.WriteLine("CanRead: " + info.CanRead);
Console.WriteLine("ProjectApplicationInfo: " + info.ProjectApplicationInfo);
Console.WriteLine("ProjectFileFormat: " + info.ProjectFileFormat);
```

### Voir aussi

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


