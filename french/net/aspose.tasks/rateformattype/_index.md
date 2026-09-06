---
title: "Énumération RateFormatType"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Énumération Aspose.Tasks.RateFormatType. Spécifie les unités utilisées par Microsoft Project pour afficher un taux."
type: docs
weight: 1640
url: /fr/net/aspose.tasks/rateformattype/
---
## RateFormatType enumeration

Spécifie les unités utilisées par Microsoft Project pour afficher un taux.

```csharp
public enum RateFormatType
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| Undefined | `-1` | La valeur n'était pas définie dans le fichier de projet original. |
| Minute | `0` | Minute ("min") |
| Hour | `1` | Heure ("hr") |
| Day | `2` | Jour ("day") |
| Week | `3` | Semaine ("wk") |
| Month | `4` | Mois ("mo") |
| Year | `5` | Année ("yr") |
| MaterialResourceRate | `6` | Taux de ressource matérielle (vide) |

## Remarques

Lors de l'exportation vers XML, les valeurs Undefined seront éliminées du XML résultant.

## Exemples

Montre comment lire/écrire la propriété Rsc.StandardRateFormat.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.StandardRateFormat, RateFormatType.Hour);

Console.WriteLine("Standard Rate Format: " + resource.Get(Rsc.StandardRateFormat));
```

### Voir aussi

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


