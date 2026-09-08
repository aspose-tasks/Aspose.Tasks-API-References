---
title: "Duration.GetHashCode"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Duration-methode. Retourneert een hashcode‑waarde voor dit object"
type: docs
weight: 90
url: /nl/net/aspose.tasks/duration/gethashcode/
---
## Duration.GetHashCode method

Retourneert een hashcode‑waarde voor dit object.

```csharp
public override int GetHashCode()
```

### Retourwaarde

retourneert een hashcode‑waarde voor deze duur‑instantie.

## Voorbeelden

Toont hoe een hashcode van een duur te verkrijgen.

```csharp
var project = new Project();

var duration1 = project.GetDuration(1, TimeUnitType.Day);
var duration2 = project.GetDuration(1, TimeUnitType.Day);
var duration3 = project.GetDuration(1, TimeUnitType.Hour);

// de hashcode van een kalender is gebaseerd op het type tijdseenheid en de initiële waarde van de duur
// dus de volgende hashcodes zijn gelijk
Console.WriteLine("Duration 1 Hash Code: {0}", duration1.GetHashCode());
Console.WriteLine("Duration 2 Hash Code: {0}", duration2.GetHashCode());
Console.WriteLine("Are duration's hash codes of duration 1 and duration 2 equal: {0}", duration1.GetHashCode().Equals(duration2.GetHashCode()));

// maar hashcodes van duur 1 en 3 zijn dat niet
Console.WriteLine("Duration 1 Hash Code: {0}", duration1.GetHashCode());
Console.WriteLine("Duration 3 Hash Code: {0}", duration3.GetHashCode());
Console.WriteLine("Are duration's hash codes of duration 1 and duration 2 equal: {0}", duration1.GetHashCode().Equals(duration3.GetHashCode()));
```

### Zie ook

* struct [Duration](../)
* namespace [Aspose.Tasks](../../duration/)
* assembly [Aspose.Tasks](../../../)


