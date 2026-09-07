---
title: "Duration.op_Inequality"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Metodo Duration. Restituisce un valore che indica se questa istanza non è uguale a un oggetto specificato"
type: docs
weight: 150
url: /it/net/aspose.tasks/duration/op_inequality/
---
## Duration Inequality operator

Restituisce un valore che indica se questa istanza non è uguale a un oggetto specificato.

```csharp
public static bool operator !=(Duration a, Duration b)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| a | Durata | La prima durata. |
| b | Durata | La seconda durata. |

### Valore di ritorno

un valore che indica se questa istanza non è uguale a un oggetto specificato

## Esempi

Mostra come verificare l'uguaglianza della durata.

```csharp
var project = new Project();

var duration1 = project.GetDuration(1, TimeUnitType.Day);
var duration2 = project.GetDuration(1, TimeUnitType.Day);
var duration3 = project.GetDuration(1, TimeUnitType.Hour);

// l'uguaglianza della durata è verificata rispetto al timespan sottostante
Console.WriteLine("Duration 1: " + duration1.TimeSpan);
Console.WriteLine("Duration 2: " + duration2.TimeSpan);
Console.WriteLine("Duration 3: " + duration3.TimeSpan);
Console.WriteLine("Are durations 1 and 2 equal: " + duration1.Equals(duration2));
Console.WriteLine("Are durations 1 and 3 equal: " + duration1.Equals(duration3));
```

### Vedi anche

* struct [Duration](../)
* namespace [Aspose.Tasks](../../duration/)
* assembly [Aspose.Tasks](../../../)


