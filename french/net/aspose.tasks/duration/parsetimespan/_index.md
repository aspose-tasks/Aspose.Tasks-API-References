---
title: "Duration.ParseTimeSpan"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Méthode Duration. Analyse la chaîne de durée au format PTHMS."
type: docs
weight: 130
url: /fr/net/aspose.tasks/duration/parsetimespan/
---
## Duration.ParseTimeSpan method

Analyse la chaîne de durée au format "PT--H--M--S--".

```csharp
public static TimeSpan ParseTimeSpan(string value)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| value | Chaîne | la chaîne spécifiée à analyser. |

### Valeur de retour

renvoie une instance analysée de la structure [`TimeSpan`](../timespan/).

## Exemples

Montre comment convertir une chaîne en intervalle de temps.

```csharp
var timeSpan = Duration.ParseTimeSpan("PT1H10M30S");
Console.WriteLine("The parsed time span: " + timeSpan);
```

### Voir aussi

* struct [Duration](../)
* namespace [Aspose.Tasks](../../duration/)
* assembly [Aspose.Tasks](../../../)


