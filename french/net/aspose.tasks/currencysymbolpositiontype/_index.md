---
title: "Énumération CurrencySymbolPositionType"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Énumération Aspose.Tasks.CurrencySymbolPositionType. Spécifie la position d’un symbole monétaire"
type: docs
weight: 370
url: /fr/net/aspose.tasks/currencysymbolpositiontype/
---
## CurrencySymbolPositionType enumeration

Spécifie la position du symbole monétaire.

```csharp
public enum CurrencySymbolPositionType
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| Undefined | `-1` | Indique que la valeur indéfinie signifie que le champ n'était pas défini dans le fichier de projet original. |
| Before | `0` | Indique le type de position du symbole monétaire Avant. |
| After | `1` | Indique le type de position du symbole monétaire Après. |
| BeforeWithSpace | `2` | Indique le type de position du symbole monétaire AvantAvecEspace. |
| AfterWithSpace | `3` | Indique le type de position du symbole monétaire AprèsAvecEspace. |

## Remarques

Lors de l'exportation vers XML, les valeurs Undefined seront éliminées du XML résultant.

## Exemples

Montre comment spécifier le placement du symbole monétaire (CurrencySymbolPositionType.Before).

```csharp
var project = new Project(DataDir + "Project2.mpp");
// définir le placement du symbole monétaire
// Avant, sans espace ($0).
project.Set(Prj.CurrencySymbolPosition, CurrencySymbolPositionType.Before);
// travailler avec le projet...
```

### Voir aussi

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


