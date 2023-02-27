---
title: TaskLink.LinkLagTimeSpan
second_title: Riferimento all'API di Aspose.Tasks per .NET
description: TaskLink proprietà. Ottiene o imposta la durata del ritardo a seconda di LagFormat.
type: docs
weight: 50
url: /it/net/aspose.tasks/tasklink/linklagtimespan/
---
## TaskLink.LinkLagTimeSpan property

Ottiene o imposta la durata del ritardo, a seconda di LagFormat.

```csharp
public TimeSpan LinkLagTimeSpan { get; set; }
```

### Eccezioni

| eccezione | condizione |
| --- | --- |
| ArgumentException | Quando si tenta di impostare il valore per TaskLinks dove LagFormat è TimeUnitType.Percent. |

### Osservazioni

Il link lag può essere un valore percentuale (LagFormat è TimeUnitType.Percent). In questo caso la durata è calcolata come percentuale della durata di PredTask. Altrimenti il metodo restituisce il valore TimeSpan che rappresenta il lag di TaskLink.

### Guarda anche

* class [TaskLink](../)
* spazio dei nomi [Aspose.Tasks](../../tasklink/)
* assemblea [Aspose.Tasks](../../../)


