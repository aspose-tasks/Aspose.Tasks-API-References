---
title: "FieldHelper.GetDefaultTaskFieldTitle"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Metodo FieldHelper. Restituisce un titolo predefinito del campo attività specifico"
type: docs
weight: 20
url: /it/net/aspose.tasks.util/fieldhelper/getdefaulttaskfieldtitle/
---
## FieldHelper.GetDefaultTaskFieldTitle method

Restituisce un titolo predefinito del campo attività specifico.

```csharp
public static string GetDefaultTaskFieldTitle(TaskKey taskKey)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| taskKey | TaskKey | Campo attività per ottenere un titolo predefinito. |

### Valore di ritorno

Un titolo predefinito del campo attività specifico se il campo può essere visualizzato nella vista di MS Project, altrimenti null.

## Esempi

Mostra come ottenere il titolo predefinito del campo per il campo attività specifico.

```csharp
Console.WriteLine("Title for Tsk.ActualCost: " + FieldHelper.GetDefaultTaskFieldTitle(Tsk.ActualCost.KeyType));
Console.WriteLine("Title for Tsk.PercentWorkComplete: " + FieldHelper.GetDefaultTaskFieldTitle(Tsk.PercentWorkComplete.KeyType));
```

### Vedi anche

* enum [TaskKey](../../../aspose.tasks/taskkey/)
* class [FieldHelper](../)
* namespace [Aspose.Tasks.Util](../../fieldhelper/)
* assembly [Aspose.Tasks](../../../)


