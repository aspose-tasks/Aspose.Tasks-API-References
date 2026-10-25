---
title: "Classe PrimaveraXmlReader"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Classe Aspose.Tasks.PrimaveraXmlReader. Représente un lecteur qui permet de récupérer les UID de projet à partir d'un fichier Primavera Xml"
type: docs
weight: 1400
url: /fr/net/aspose.tasks/primaveraxmlreader/
---
## PrimaveraXmlReader class

Représente un lecteur qui permet de récupérer les UID de projet à partir d'un fichier Primavera XML.

```csharp
public class PrimaveraXmlReader : PrimaveraBaseReader
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [PrimaveraXmlReader](primaveraxmlreader/#constructor)(Stream) | Initialise une nouvelle instance de la classe `PrimaveraXmlReader`. |
| [PrimaveraXmlReader](primaveraxmlreader/#constructor_1)(string) | Initialise une nouvelle instance de la classe `PrimaveraXmlReader`. |

## Méthodes

| Nom | Description |
| --- | --- |
| [GetProjectInfos](../../aspose.tasks/primaverabasereader/getprojectinfos/)() | Renvoie une liste des objets d'informations courtes du projet. |
| [GetProjectUids](../../aspose.tasks/primaverabasereader/getprojectuids/)() | Retourner une liste des identifiants uniques des projets. |
| virtual [LoadProject](../../aspose.tasks/primaverabasereader/loadproject/)(int) | Charge le projet avec l'identifiant unique spécifié. |

## Exemples

Montre comment examiner les informations des projets courts à partir d'un fichier Primavera XML.

```csharp
var reader = new PrimaveraXmlReader(DataDir + "MultiprojectWithExternal.xml");
var projectInfos = reader.GetProjectInfos();
foreach (var info in projectInfos)
{
    Console.WriteLine("{0} - '{1}' - {2}", info.Uid, info.Name, info.ExportFlag);
}
```

### Voir aussi

* class [PrimaveraBaseReader](../primaverabasereader/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


