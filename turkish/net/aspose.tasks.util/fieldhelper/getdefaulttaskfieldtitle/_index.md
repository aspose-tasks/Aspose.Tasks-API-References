---
title: "FieldHelper.GetDefaultTaskFieldTitle"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "FieldHelper yöntemi. Belirli görev alanının varsayılan başlığını döndürür."
type: docs
weight: 20
url: /tr/net/aspose.tasks.util/fieldhelper/getdefaulttaskfieldtitle/
---
## FieldHelper.GetDefaultTaskFieldTitle method

Belirli görev alanının varsayılan başlığını döndürür.

```csharp
public static string GetDefaultTaskFieldTitle(TaskKey taskKey)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| taskKey | TaskKey | Varsayılan bir başlık almak için görev alanı. |

### Dönüş Değeri

Alan MS Project görünümünde görüntülenebiliyorsa, belirli görev alanının varsayılan başlığı; aksi takdirde null.

## Örnekler

Belirli görevin alanı için varsayılan alan başlığının nasıl alınacağını gösterir.

```csharp
Console.WriteLine("Title for Tsk.ActualCost: " + FieldHelper.GetDefaultTaskFieldTitle(Tsk.ActualCost.KeyType));
Console.WriteLine("Title for Tsk.PercentWorkComplete: " + FieldHelper.GetDefaultTaskFieldTitle(Tsk.PercentWorkComplete.KeyType));
```

### Ayrıca Bakınız

* enum [TaskKey](../../../aspose.tasks/taskkey/)
* class [FieldHelper](../)
* namespace [Aspose.Tasks.Util](../../fieldhelper/)
* assembly [Aspose.Tasks](../../../)


