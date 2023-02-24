---
title: TaskLink.LinkLagTimeSpan
second_title: Aspose.Tasks für .NET-API-Referenz
description: TaskLink eigendom. Ruft die Verzögerungsdauer ab oder legt sie fest abhängig vom LagFormat.
type: docs
weight: 50
url: /de/net/aspose.tasks/tasklink/linklagtimespan/
---
## TaskLink.LinkLagTimeSpan property

Ruft die Verzögerungsdauer ab oder legt sie fest, abhängig vom LagFormat.

```csharp
public TimeSpan LinkLagTimeSpan { get; set; }
```

### Ausnahmen

| Ausnahme | Bedingung |
| --- | --- |
| ArgumentException | Beim Versuch, den Wert für TaskLinks festzulegen, wobei LagFormat TimeUnitType.Percent ist. |

### Bemerkungen

Die Verbindungsverzögerung kann ein Prozentwert sein (LagFormat ist TimeUnitType.Percent). In diesem Fall wird die Dauer als Prozentsatz der Dauer von PredTask berechnet. Andernfalls gibt die Methode den TimeSpan-Wert zurück, der die Verzögerung von TaskLink darstellt.

### Siehe auch

* class [TaskLink](../)
* namensraum [Aspose.Tasks](../../tasklink/)
* Montage [Aspose.Tasks](../../../)


