---
title: "Duration.IsElapsed"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Duration-eigenschap. Haalt een waarde op die aangeeft of de tijdseenheid verstreken is. De vlag die bepaalt of deze Duration‑instantie verstreken is"
type: docs
weight: 20
url: /nl/net/aspose.tasks/duration/iselapsed/
---
## Duration.IsElapsed property

Haalt een waarde op die aangeeft of de tijdseenheid verstreken is. De vlag die bepaalt of deze Duration‑instantie verstreken is.

```csharp
public bool IsElapsed { get; }
```

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

* struct [Duration](../)
* namespace [Aspose.Tasks](../../duration/)
* assembly [Aspose.Tasks](../../../)


