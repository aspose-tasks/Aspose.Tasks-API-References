---
title: "Classe PrimaveraXerReader"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Classe Aspose.Tasks.PrimaveraXerReader. Représente un lecteur permettant de lire les UID de projet depuis un fichier Primavera XER"
type: docs
weight: 1390
url: /fr/net/aspose.tasks/primaveraxerreader/
---
## PrimaveraXerReader class

Représente un lecteur permettant de lire les UID de projet à partir d'un fichier Primavera XER

```csharp
public sealed class PrimaveraXerReader : PrimaveraBaseReader
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [PrimaveraXerReader](primaveraxerreader/#constructor)(Stream) | Initialise une nouvelle instance de la classe `PrimaveraXerReader`. |
| [PrimaveraXerReader](primaveraxerreader/#constructor_1)(string) | Initialise une nouvelle instance de la classe `PrimaveraXerReader`. |

## Méthodes

| Nom | Description |
| --- | --- |
| [GetProjectInfos](../../aspose.tasks/primaverabasereader/getprojectinfos/)() | Renvoie une liste des objets d'informations courtes du projet. |
| [GetProjectUids](../../aspose.tasks/primaverabasereader/getprojectuids/)() | Retourner une liste des identifiants uniques des projets. |
| virtual [LoadProject](../../aspose.tasks/primaverabasereader/loadproject/)(int) | Charge le projet avec l'identifiant unique spécifié. |

## Exemples

Montre comment examiner les informations des projets courts à partir d'un fichier Primavera XER.

```csharp
var reader = new PrimaveraXerReader(DataDir + "MultiprojectWithExternal.xer");
var projectInfos = reader.GetProjectInfos();
foreach (var info in projectInfos)
{
    Console.WriteLine("{0} - '{1}' - {2}", info.Uid, info.Name, info.ExportFlag);
}

var project = reader.LoadProject(5494);

Console.WriteLine("Loaded project '{0}' with Uid {1}", project.Name, project.Uid);
```

### Voir aussi

* class [PrimaveraBaseReader](../primaverabasereader/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


