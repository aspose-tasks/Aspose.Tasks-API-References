---
title: Struct Duration
second_title: Référence de l'API Aspose.Tasks pour .NET
description: Aspose.Tasks.Duration structure. Représente la durée dans un projet.
type: docs
weight: 470
url: /fr/net/aspose.tasks/duration/
---
## Duration structure

Représente la durée dans un projet.

```csharp
public struct Duration : IEquatable<Duration>
```

## Propriétés

| Nom | La description |
| --- | --- |
| [IsElapsed](../../aspose.tasks/duration/iselapsed/) { get; } | Obtient une valeur indiquant si l'unité de temps est écoulée. L'indicateur qui détermine si cette instance Duration est écoulée. |
| [IsEstimated](../../aspose.tasks/duration/isestimated/) { get; } | Obtient une valeur indiquant si l'unité de temps est estimée. L'indicateur qui détermine si cette instance Duration est estimée. |
| [TimeSpan](../../aspose.tasks/duration/timespan/) { get; } | Obtient[`TimeSpan`](./timespan/) instance de cet objet Durée. L'instance TimeSpan de cet objet Duration. |
| [TimeUnit](../../aspose.tasks/duration/timeunit/) { get; } | Obtient le type d'unité de temps pour cet objet. Type d'unité de temps de cette instance Duration. |

## Méthodes

| Nom | La description |
| --- | --- |
| static [Parse](../../aspose.tasks/duration/parse/)(Project, string) | Convertit la chaîne spécifiée en instance de`Duration` structure. |
| [Add](../../aspose.tasks/duration/add/#add_1)(double) | Ajoute la valeur double spécifiée à cette durée. |
| [Add](../../aspose.tasks/duration/add/#add)(Duration) | Ajoute la durée spécifiée à cette durée. |
| [Convert](../../aspose.tasks/duration/convert/)(TimeUnitType) | Convertit l'objet Durée en une autre durée avec des unités de temps spécifiées. |
| [Equals](../../aspose.tasks/duration/equals/#equals)(Duration) | Renvoie une valeur indiquant si cette instance est égale à un objet spécifié. |
| override [Equals](../../aspose.tasks/duration/equals/#equals_1)(object) | Renvoie une valeur indiquant si cette instance est égale à un objet spécifié. |
| override [GetHashCode](../../aspose.tasks/duration/gethashcode/)() | Renvoie une valeur de code de hachage pour cet objet. |
| [Subtract](../../aspose.tasks/duration/subtract/#subtract_1)(double) | Soustrait la valeur double spécifiée de cette instance de durée. |
| [Subtract](../../aspose.tasks/duration/subtract/#subtract)(Duration) | Soustrait la durée spécifiée de cette instance de durée. |
| [ToDouble](../../aspose.tasks/duration/todouble/)() | Convertit l'objet Durée enDouble valeur. |
| override [ToString](../../aspose.tasks/duration/tostring/)() | Renvoie une représentation sous forme de chaîne de cette instance. |
| static [ParseTimeSpan](../../aspose.tasks/duration/parsetimespan/)(string) | Analyse la chaîne de durée au format "PT--H--M--S--". |
| [operator ==](../../aspose.tasks/duration/op_equality/) | Renvoie une valeur indiquant si cette instance est égale à un objet spécifié. |
| [operator !=](../../aspose.tasks/duration/op_inequality/) | Renvoie une valeur indiquant si cette instance n'est pas égale à un objet spécifié. |

### Voir également

* espace de noms [Aspose.Tasks](../../aspose.tasks/)
* Assemblée [Aspose.Tasks](../../)


