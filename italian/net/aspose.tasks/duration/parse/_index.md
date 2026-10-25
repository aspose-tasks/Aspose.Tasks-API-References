---
title: "Duration.Parse"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Metodo Duration. Converte la stringa specificata nell'istanza della struttura Duration"
type: docs
weight: 10
url: /it/net/aspose.tasks/duration/parse/
---
## Duration.Parse method

Converte la stringa specificata nell'istanza della struttura [`Duration`](../).

```csharp
public static Duration Parse(Project p, string value)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| p | Project | l'istanza specificata della classe [`Project`](../../project/) per convertire la durata. |
| valore | Stringa | la stringa specificata da convertire. |

### Valore di ritorno

Restituisce l'istanza convertita della struttura [`Duration`](../).

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

* class [Project](../../project/)
* struct [Duration](../)
* namespace [Aspose.Tasks](../../duration/)
* assembly [Aspose.Tasks](../../../)


