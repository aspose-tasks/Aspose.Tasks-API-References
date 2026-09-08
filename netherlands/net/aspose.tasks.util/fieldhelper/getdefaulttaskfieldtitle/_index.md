---
title: "FieldHelper.GetDefaultTaskFieldTitle"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "FieldHelper-methode. Retourneert een standaardtitel van het specifieke taakveld"
type: docs
weight: 20
url: /nl/net/aspose.tasks.util/fieldhelper/getdefaulttaskfieldtitle/
---
## FieldHelper.GetDefaultTaskFieldTitle method

Retourneert een standaardtitel van het specifieke taakveld.

```csharp
public static string GetDefaultTaskFieldTitle(TaskKey taskKey)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| taskKey | TaskKey | Taakveld om een standaardtitel te verkrijgen. |

### Retourwaarde

Een standaardtitel van het specifieke taakveld als het veld kan worden weergegeven in de weergave van MS Project, anders null.

## Voorbeelden

Toont hoe een standaard veldtitel te verkrijgen voor het specifieke taakveld.

```csharp
Console.WriteLine("Title for Tsk.ActualCost: " + FieldHelper.GetDefaultTaskFieldTitle(Tsk.ActualCost.KeyType));
Console.WriteLine("Title for Tsk.PercentWorkComplete: " + FieldHelper.GetDefaultTaskFieldTitle(Tsk.PercentWorkComplete.KeyType));
```

### Zie ook

* enum [TaskKey](../../../aspose.tasks/taskkey/)
* class [FieldHelper](../)
* namespace [Aspose.Tasks.Util](../../fieldhelper/)
* assembly [Aspose.Tasks](../../../)


