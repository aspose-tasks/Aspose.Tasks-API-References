---
title: "Duration.IsEstimated"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Proprietà Duration. Ottiene un valore che indica se l'unità di tempo è stimata. Il flag che determina se questa istanza Duration è stimata"
type: docs
weight: 30
url: /it/net/aspose.tasks/duration/isestimated/
---
## Duration.IsEstimated property

Ottiene un valore che indica se l'unità di tempo è stimata. Il flag che determina se questa istanza di Duration è stimata.

```csharp
public bool IsEstimated { get; }
```

## Esempi

Mostra come analizzare una stringa da una stringa formattata specialmente.

```csharp
var project = new Project();

// esempi di durate:
// "1d", "1dy", "1d?", "1day", "1 dy", "1 edy? ", "8hr", "8 hour", "8hours", "0.2w?", "0.2wk", "0.2 eweek", "0.2ew?"
// dove 1 - numero di elementi (giorno, settimana, ecc.), d - giorno (h - ora, w - settimana) ? - flag stimato, e - flag trascorso

// prova a analizzare una durata stimata
var duration1 = Duration.Parse(project, "1d?");
Console.WriteLine("The parsed time span: " + duration1.TimeSpan);
Console.WriteLine("The parsed time unit: " + duration1.TimeUnit);
Console.WriteLine("Is estimated duration?: " + duration1.IsEstimated);
Console.WriteLine("Is elapsed duration?: " + duration1.IsElapsed);
Console.WriteLine();

// prova a analizzare una durata stimata
var duration2 = Duration.Parse(project, "0.2 eweek");
Console.WriteLine("The parsed time span: " + duration2.TimeSpan);
Console.WriteLine("The parsed time unit: " + duration2.TimeUnit);
Console.WriteLine("Is estimated duration?: " + duration2.IsEstimated);
Console.WriteLine("Is elapsed duration?: " + duration2.IsElapsed);
```

### Vedi anche

* struct [Duration](../)
* namespace [Aspose.Tasks](../../duration/)
* assembly [Aspose.Tasks](../../../)


