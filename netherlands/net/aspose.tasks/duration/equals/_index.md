---
title: "Duration.Equals"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Duration-methode. Retourneert een waarde die aangeeft of deze instantie gelijk is aan een opgegeven object"
type: docs
weight: 80
url: /nl/net/aspose.tasks/duration/equals/
---
## Equals(Duration) {#equals}

Retourneert een waarde die aangeeft of deze instantie gelijk is aan een opgegeven object.

```csharp
public bool Equals(Duration other)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| anders | Duur | Het object om te vergelijken met deze instantie. |

### Retourwaarde

Retourneert **True** als een andere Duration‑instantie dezelfde TimeSpan‑ en TimeUnit‑waarden heeft als deze instantie; anders **false**.

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

---

## Equals(object) {#equals_1}

Retourneert een waarde die aangeeft of deze instantie gelijk is aan een opgegeven object.

```csharp
public override bool Equals(object obj)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| obj | Object | Het object om te vergelijken met deze instantie. |

### Retourwaarde

**True** if the specified object is a Duration that has the same TimeSpan and TimeUnit values as this instance; otherwise, **false**.

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


