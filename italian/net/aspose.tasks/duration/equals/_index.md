---
title: "Duration.Equals"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Metodo Duration. Restituisce un valore che indica se questa istanza è uguale a un oggetto specificato"
type: docs
weight: 80
url: /it/net/aspose.tasks/duration/equals/
---
## Equals(Duration) {#equals}

Restituisce un valore che indica se questa istanza è uguale a un oggetto specificato.

```csharp
public bool Equals(Duration other)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| altro | Durata | L'oggetto da confrontare con questa istanza. |

### Valore di ritorno

Restituisce **True** se un'altra istanza Duration ha gli stessi valori di TimeSpan e TimeUnit di questa istanza; altrimenti, **false**.

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

---

## Equals(object) {#equals_1}

Restituisce un valore che indica se questa istanza è uguale a un oggetto specificato.

```csharp
public override bool Equals(object obj)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| obj | Oggetto | L'oggetto da confrontare con questa istanza. |

### Valore di ritorno

**True** if the specified object is a Duration that has the same TimeSpan and TimeUnit values as this instance; otherwise, **false**.

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


