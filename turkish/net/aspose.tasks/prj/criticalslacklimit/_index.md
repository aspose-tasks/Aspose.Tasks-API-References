---
title: "Prj.CriticalSlackLimit"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Prj alanı. Toplam gecikme süresi bu gün sayısına eşit veya daha az ise MS Project tarafından görevler kritik olarak kabul edilir"
type: docs
weight: 140
url: /tr/net/aspose.tasks/prj/criticalslacklimit/
---
## Prj.CriticalSlackLimit field

Toplam gecikme süresi bu gün sayısına eşit veya daha az ise MS Project görevleri kritik olarak kabul eder.

```csharp
public static readonly Key<int, PrjKey> CriticalSlackLimit;
```

## Örnekler

Prj.CriticalSlackLimit özelliğinin nasıl okunup yazılacağını gösterir.

```csharp
var project = new Project();

project.Set(Prj.CriticalSlackLimit, 2);

Console.WriteLine("Critical Slack Limit: " + project.Get(Prj.CriticalSlackLimit));
```

### Ayrıca Bakınız

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


