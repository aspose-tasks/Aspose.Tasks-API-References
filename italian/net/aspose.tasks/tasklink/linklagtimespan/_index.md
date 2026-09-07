---
title: "TaskLink.LinkLagTimeSpan"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Proprietà TaskLink. Ottiene o imposta la durata del ritardo in base a LagFormat"
type: docs
weight: 50
url: /it/net/aspose.tasks/tasklink/linklagtimespan/
---
## TaskLink.LinkLagTimeSpan property

Ottiene o imposta la durata del ritardo, a seconda del LagFormat.

```csharp
public TimeSpan LinkLagTimeSpan { get; set; }
```

### Eccezioni

| eccezione | condizione |
| --- | --- |
| ArgumentException | Quando si tenta di impostare il valore per i TaskLink in cui LagFormat è TimeUnitType.Percent. |

## Osservazioni

Il ritardo del collegamento può essere un valore percentuale (LagFormat è TimeUnitType.Percent). In questo caso la durata è calcolata come percentuale della durata di PredTask. Altrimenti il metodo restituisce un valore TimeSpan che rappresenta il ritardo del TaskLink.

### Vedi anche

* class [TaskLink](../)
* namespace [Aspose.Tasks](../../tasklink/)
* assembly [Aspose.Tasks](../../../)


