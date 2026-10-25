---
title: "Duration.op_Equality"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Duration-methode. Retourneert een waarde die aangeeft of deze instantie gelijk is aan een opgegeven object"
type: docs
weight: 140
url: /nl/net/aspose.tasks/duration/op_equality/
---
## Duration Equality operator

Retourneert een waarde die aangeeft of deze instantie gelijk is aan een opgegeven object.

```csharp
public static bool operator ==(Duration a, Duration b)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| een | Duur | De eerste duur. |
| b | Duur | De tweede duur. |

### Retourwaarde

een waarde die aangeeft of deze instantie gelijk is aan een opgegeven object

## Voorbeelden

Toont hoe duurgelijkheid te controleren.

```csharp
var project = new Project();

var duration1 = project.GetDuration(1, TimeUnitType.Day);
var duration2 = project.GetDuration(1, TimeUnitType.Day);
var duration3 = project.GetDuration(1, TimeUnitType.Hour);

// de gelijkheid van de duur wordt gecontroleerd ten opzichte van de onderliggende timespan
Console.WriteLine("Duration 1: " + duration1.TimeSpan);
Console.WriteLine("Duration 2: " + duration2.TimeSpan);
Console.WriteLine("Duration 3: " + duration3.TimeSpan);
Console.WriteLine("Are durations 1 and 2 equal: " + duration1.Equals(duration2));
Console.WriteLine("Are durations 1 and 3 equal: " + duration1.Equals(duration3));
```

### Zie ook

* struct [Duration](../)
* namespace [Aspose.Tasks](../../duration/)
* assembly [Aspose.Tasks](../../../)


