---
title: "Project.GetBaselineSaveTime"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Méthode Project. Retourne l'heure d'enregistrement de la ligne de base"
type: docs
weight: 1090
url: /fr/net/aspose.tasks/project/getbaselinesavetime/
---
## Project.GetBaselineSaveTime method

Renvoie le temps d’enregistrement de la ligne de base.

```csharp
public DateTime GetBaselineSaveTime(BaselineType baselineNumber)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| baselineNumber | BaselineType | Le numéro de la ligne de base [`BaselineType`](../../baselinetype/). |

### Valeur de retour

La dernière date et heure de sauvegarde de la ligne de base.

## Remarques

Retourne DateTime.MinValue si la ligne de base n'a pas été enregistrée.

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


