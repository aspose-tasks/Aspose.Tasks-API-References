---
title: "WorkingTime.Equals"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "WorkingTime method. Controleert of de objecten gelijk zijn"
type: docs
weight: 40
url: /nl/net/aspose.tasks/workingtime/equals/
---
## WorkingTime.Equals method

Controleert of de objecten gelijk zijn.

```csharp
public override bool Equals(object obj)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| obj | Object | Tweede object om te vergelijken. |

### Retourwaarde

True als de objecten gelijk zijn, false anders.

## Voorbeelden

Toont hoe de gelijkheid van werktijd te controleren.

```csharp
var workingTime1 = new WorkingTime(9, 12);
var workingTime2 = new WorkingTime(13, 17);

// De gelijkheid van kalenders wordt gecontroleerd aan de hand van de van- en tot-datums van de werktijd.
Console.WriteLine("Working Time 1 (From): " + workingTime1.From);
Console.WriteLine("Working Time 1 (To): " + workingTime1.To);

Console.WriteLine("Working Time 2 (From): " + workingTime2.From);
Console.WriteLine("Working Time 2 (To): " + workingTime2.To);
Console.WriteLine("Are working times equal: " + workingTime1.Equals(workingTime2));
```

### Zie ook

* class [WorkingTime](../)
* namespace [Aspose.Tasks](../../workingtime/)
* assembly [Aspose.Tasks](../../../)


