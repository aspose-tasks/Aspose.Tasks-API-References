---
title: "Duration.GetHashCode"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Metodo Duration. Restituisce un valore di hash code per questo oggetto."
type: docs
weight: 90
url: /it/net/aspose.tasks/duration/gethashcode/
---
## Duration.GetHashCode method

Restituisce un valore di hash code per questo oggetto.

```csharp
public override int GetHashCode()
```

### Valore di ritorno

restituisce un valore di hash code per questa istanza di durata.

## Esempi

Mostra come ottenere un hash code di una durata.

```csharp
var project = new Project();

var duration1 = project.GetDuration(1, TimeUnitType.Day);
var duration2 = project.GetDuration(1, TimeUnitType.Day);
var duration3 = project.GetDuration(1, TimeUnitType.Hour);

// l'hash code di un calendario è basato sul tipo di unità di tempo e sul valore iniziale della durata.
// quindi i successivi hash code sono uguali.
Console.WriteLine("Duration 1 Hash Code: {0}", duration1.GetHashCode());
Console.WriteLine("Duration 2 Hash Code: {0}", duration2.GetHashCode());
Console.WriteLine("Are duration's hash codes of duration 1 and duration 2 equal: {0}", duration1.GetHashCode().Equals(duration2.GetHashCode()));

// ma gli hash code della durata 1 e 3 non lo sono.
Console.WriteLine("Duration 1 Hash Code: {0}", duration1.GetHashCode());
Console.WriteLine("Duration 3 Hash Code: {0}", duration3.GetHashCode());
Console.WriteLine("Are duration's hash codes of duration 1 and duration 2 equal: {0}", duration1.GetHashCode().Equals(duration3.GetHashCode()));
```

### Vedi anche

* struct [Duration](../)
* namespace [Aspose.Tasks](../../duration/)
* assembly [Aspose.Tasks](../../../)


