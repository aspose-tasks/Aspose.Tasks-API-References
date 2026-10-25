---
title: "Duration.op_Inequality"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Méthode Duration. Renvoie une valeur indiquant si cette instance n'est pas égale à un objet spécifié"
type: docs
weight: 150
url: /fr/net/aspose.tasks/duration/op_inequality/
---
## Duration Inequality operator

Renvoie une valeur indiquant si cette instance n'est pas égale à un objet spécifié.

```csharp
public static bool operator !=(Duration a, Duration b)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| a | Duration | La première durée. |
| b | Duration | La deuxième durée. |

### Valeur de retour

une valeur indiquant si cette instance n'est pas égale à un objet spécifié.

## Exemples

Montre comment vérifier l'égalité des durées.

```csharp
var project = new Project();

var duration1 = project.GetDuration(1, TimeUnitType.Day);
var duration2 = project.GetDuration(1, TimeUnitType.Day);
var duration3 = project.GetDuration(1, TimeUnitType.Hour);

// l'égalité de la durée est vérifiée par rapport au timespan sous-jacent
Console.WriteLine("Duration 1: " + duration1.TimeSpan);
Console.WriteLine("Duration 2: " + duration2.TimeSpan);
Console.WriteLine("Duration 3: " + duration3.TimeSpan);
Console.WriteLine("Are durations 1 and 2 equal: " + duration1.Equals(duration2));
Console.WriteLine("Are durations 1 and 3 equal: " + duration1.Equals(duration3));
```

### Voir aussi

* struct [Duration](../)
* namespace [Aspose.Tasks](../../duration/)
* assembly [Aspose.Tasks](../../../)


