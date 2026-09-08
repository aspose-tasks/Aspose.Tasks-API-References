---
title: "Duration.Parse"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Duration-methode. Converteert de opgegeven string naar de instantie van de Duration-structuur"
type: docs
weight: 10
url: /nl/net/aspose.tasks/duration/parse/
---
## Duration.Parse method

Converteert de opgegeven string naar de instantie van [`Duration`](../) struct.

```csharp
public static Duration Parse(Project p, string value)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| p | Project | de opgegeven instantie van [`Project`](../../project/) klasse om de duur te converteren. |
| value | String | de opgegeven string om te converteren. |

### Retourwaarde

Retourneert de geconverteerde instantie van [`Duration`](../) struct.

## Voorbeelden

Toont hoe een tekenreeks te parseren vanuit een speciaal opgemaakte tekenreeks.

```csharp
var project = new Project();

// voorbeelden van duurwaarden:
// "1d", "1dy", "1d?", "1day", "1 dy", "1 edy? ", "8hr", "8 hour", "8hours", "0.2w?", "0.2wk", "0.2 eweek", "0.2ew?"
// waar 1 - aantal items (dag, week, enz.), d - dag (h - uur, w - week) ? - geschatte vlag, e - verstreken vlag

// probeer een geschatte duur te parseren
var duration1 = Duration.Parse(project, "1d?");
Console.WriteLine("The parsed time span: " + duration1.TimeSpan);
Console.WriteLine("The parsed time unit: " + duration1.TimeUnit);
Console.WriteLine("Is estimated duration?: " + duration1.IsEstimated);
Console.WriteLine("Is elapsed duration?: " + duration1.IsElapsed);
Console.WriteLine();

// probeer een geschatte duur te parseren
var duration2 = Duration.Parse(project, "0.2 eweek");
Console.WriteLine("The parsed time span: " + duration2.TimeSpan);
Console.WriteLine("The parsed time unit: " + duration2.TimeUnit);
Console.WriteLine("Is estimated duration?: " + duration2.IsEstimated);
Console.WriteLine("Is elapsed duration?: " + duration2.IsElapsed);
```

### Zie ook

* class [Project](../../project/)
* struct [Duration](../)
* namespace [Aspose.Tasks](../../duration/)
* assembly [Aspose.Tasks](../../../)


