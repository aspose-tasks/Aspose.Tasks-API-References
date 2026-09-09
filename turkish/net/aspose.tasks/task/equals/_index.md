---
title: "Task.Equals"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Task yöntemi. Bu örneğin belirtilen bir görevle eşit olup olmadığını gösteren bir değer döndürür."
type: docs
weight: 1330
url: /tr/net/aspose.tasks/task/equals/
---
## Equals(Task) {#equals}

Bu örneğin belirtilen bir görevle eşit olup olmadığını gösteren bir değer döndürür.

```csharp
public bool Equals(Task other)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| diğer | Görev | Bu örnek ile karşılaştırılacak belirtilen görev. |

### Dönüş Değeri

Belirtilen görev ve bu örnek eşit benzersiz kimliklere sahipse true döndürür.

## Örnekler

Görevin atamalarında nasıl yineleme yapılacağını gösterir.

```csharp
var project = new Project(DataDir + "BudgetWorkAndCost.mpp");

var collector = new ChildTasksCollector();
TaskUtils.Apply(project.RootTask, collector, 0);
foreach (var task in collector.Tasks)
{
    // görevin atamalarını göster
    foreach (var assignment in task.Assignments)
    {
        Console.WriteLine(assignment.ToString());
    }
}
```

### Ayrıca Bakınız

* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)

---

## Equals(object) {#equals_1}

Bu örneğin belirtilen nesneye eşit olup olmadığını gösteren bir değer döndürür.

```csharp
public override bool Equals(object obj)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| obj | Object | Bu örnek ile karşılaştırılacak belirtilen nesne. |

### Dönüş Değeri

Belirtilen görev ve bu örnek eşit benzersiz kimliklere sahipse true döndürür.

## Örnekler

Görevin atamalarında nasıl yineleme yapılacağını gösterir.

```csharp
var project = new Project(DataDir + "BudgetWorkAndCost.mpp");

var collector = new ChildTasksCollector();
TaskUtils.Apply(project.RootTask, collector, 0);
foreach (var task in collector.Tasks)
{
    // görevin atamalarını göster
    foreach (var assignment in task.Assignments)
    {
        Console.WriteLine(assignment.ToString());
    }
}
```

### Ayrıca Bakınız

* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


