---
title: "Enum EarnedValueMethodType"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Aspose.Tasks.EarnedValueMethodType enum. Spécifie la méthode utilisée pour calculer la valeur acquise"
type: docs
weight: 480
url: /fr/net/aspose.tasks/earnedvaluemethodtype/
---
## EarnedValueMethodType enumeration

Spécifie la méthode utilisée pour calculer la valeur acquise.

```csharp
public enum EarnedValueMethodType
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| Undefined | `-1` | Le champ n'était pas défini dans le fichier de projet original. |
| PercentComplete | `0` | Pourcentage achevé |
| PhysicalPercentComplete | `1` | Pourcentage physique achevé |

## Remarques

Lors de l'exportation vers XML, les valeurs Undefined seront éliminées du XML résultant.

## Exemples

Montre comment spécifier la méthode utilisée pour calculer la valeur acquise (EarnedValueMethodType.PercentComplete).

```csharp
var project = new Project(DataDir + "Project2.mpp");
// définir le type de méthode de valeur acquise sur 'PercentComplete'
project.Set(Prj.DefaultTaskEVMethod, EarnedValueMethodType.PercentComplete);
// travailler avec le projet...
```

### Voir aussi

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


