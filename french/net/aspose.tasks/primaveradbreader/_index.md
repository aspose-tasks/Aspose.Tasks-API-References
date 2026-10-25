---
title: "Classe PrimaveraDbReader"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Classe Aspose.Tasks.PrimaveraDbReader. Représente un lecteur permettant de lire les informations du projet depuis la base de données Primavera"
type: docs
weight: 1350
url: /fr/net/aspose.tasks/primaveradbreader/
---
## PrimaveraDbReader class

Représente un lecteur permettant de lire les informations du projet depuis la base de données Primavera

```csharp
public sealed class PrimaveraDbReader : PrimaveraBaseReader
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [PrimaveraDbReader](primaveradbreader/)(PrimaveraDbSettings) | Initialise une nouvelle instance de la classe [`PrimaveraXerReader`](../primaveraxerreader/). |

## Méthodes

| Nom | Description |
| --- | --- |
| [GetProjectInfos](../../aspose.tasks/primaverabasereader/getprojectinfos/)() | Renvoie une liste des objets d'informations courtes du projet. |
| [GetProjectUids](../../aspose.tasks/primaverabasereader/getprojectuids/)() | Retourner une liste des identifiants uniques des projets. |
| override [LoadProject](../../aspose.tasks/primaveradbreader/loadproject/)(int) | Charge le projet avec l'identifiant unique spécifié. |

## Exemples

Montre comment obtenir des informations brèves des projets à partir d'une base de données Primavera.

```csharp
var settings = new PrimaveraDbSettings(GetConnectionString(), 0);

var reader = new PrimaveraDbReader(settings);
var projectInfos = reader.GetProjectInfos();

foreach (var info in projectInfos)
{
    Console.WriteLine("{0} - '{1}' - '{2}'", info.Uid, info.ShortName, info.Name);
}

var firstProject = reader.LoadProject(projectInfos[0].Uid);
Console.WriteLine(firstProject.Uid);
Console.WriteLine(firstProject.Name);
Console.WriteLine(firstProject.PrimaveraProperties.ShortName);
```

### Voir aussi

* class [PrimaveraBaseReader](../primaverabasereader/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


