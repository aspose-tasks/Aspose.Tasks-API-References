---
title: "Classe PrimaveraReadOptions"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Classe Aspose.Tasks.PrimaveraReadOptions. Permet de spécifier des options supplémentaires lors de la lecture des fichiers Primavera Xml ou Primavera Xer"
type: docs
weight: 1370
url: /fr/net/aspose.tasks/primaverareadoptions/
---
## PrimaveraReadOptions class

Permet de spécifier des options supplémentaires lors de la lecture de fichiers Primavera XML ou Primavera XER.

```csharp
public class PrimaveraReadOptions
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [PrimaveraReadOptions](primaverareadoptions/)() | Initialise une nouvelle instance de la classe `PrimaveraReadOptions`. |

## Propriétés

| Nom | Description |
| --- | --- |
| [PreserveUids](../../aspose.tasks/primaverareadoptions/preserveuids/) { get; set; } | Obtient ou définit un indicateur qui spécifie si les identifiants uniques originaux des entités doivent être conservés. |
| [ProjectUid](../../aspose.tasks/primaverareadoptions/projectuid/) { get; set; } | Obtient ou définit l'UID d'un projet à lire à partir d'un fichier contenant plusieurs projets. |
| [ReadBaselineProjects](../../aspose.tasks/primaverareadoptions/readbaselineprojects/) { get; set; } | Obtient ou définit un indicateur qui spécifie si les projets de référence doivent être chargés. La valeur par défaut est true. |
| [UndefinedConstraintHandlingBehavior](../../aspose.tasks/primaverareadoptions/undefinedconstrainthandlingbehavior/) { get; set; } | Spécifie le comportement utilisé pour traiter les tâches avec des contraintes indéfinies lues à partir du format XER. |

## Exemples

Montre comment lire un projet à partir d'un fichier Primavera XML ou Primavera XER contenant plusieurs projets.

```csharp
var options = new PrimaveraReadOptions();
options.ProjectUid = 3881;

// Renvoie le projet avec un UID spécial
var project = new Project(DataDir + "PrimaveraProject.xml", options);
Console.WriteLine(project.Get(Prj.Name));
```

### Voir aussi

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


