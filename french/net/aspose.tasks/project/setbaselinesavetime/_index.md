---
title: "Project.SetBaselineSaveTime"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Méthode du projet. Définit l'heure d'enregistrement de la ligne de base"
type: docs
weight: 1260
url: /fr/net/aspose.tasks/project/setbaselinesavetime/
---
## Project.SetBaselineSaveTime method

Définit l’heure d’enregistrement de la base de référence.

```csharp
public void SetBaselineSaveTime(BaselineType baselineNumber, DateTime value)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| baselineNumber | BaselineType | Le numéro de la ligne de base [`BaselineType`](../../baselinetype/). |
| value | DateTime | La dernière date et heure de sauvegarde de la ligne de base. |

## Remarques

Définissez la valeur à DateTime.MinValue si la ligne de base n'a pas été sauvegardée.

## Exemples

Montre comment lire/écrire l'heure de sauvegarde de la ligne de base du projet.

```csharp
var project = new Project();
var baselineSave = project.GetBaselineSaveTime(BaselineType.Baseline);
Console.WriteLine("Baseline save time before: " + baselineSave);

// définir l'heure de sauvegarde de la ligne de base
project.SetBaselineSaveTime(BaselineType.Baseline, DateTime.Today);

var baselineSaveNew = project.GetBaselineSaveTime(BaselineType.Baseline);
Console.WriteLine("Baseline save time after: " + baselineSaveNew);
```

### Voir aussi

* enum [BaselineType](../../baselinetype/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


