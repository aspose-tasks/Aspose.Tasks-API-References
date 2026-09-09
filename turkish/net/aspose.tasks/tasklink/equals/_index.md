---
title: "TaskLink.Equals"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "TaskLink yöntemi. Bu örneğin belirtilen bir nesneye eşit olup olmadığını gösteren bir değer döndürür"
type: docs
weight: 90
url: /tr/net/aspose.tasks/tasklink/equals/
---
## Equals(TaskLink) {#equals}

Bu örneğin belirtilen nesneye eşit olup olmadığını gösteren bir değer döndürür.

```csharp
public bool Equals(TaskLink other)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| other | TaskLink | Bu örnek ile karşılaştırmak için belirtilen [`TaskLink`](../) sınıfının örneği. |

### Dönüş Değeri

**True** if the specified instance of the [`TaskLink`](../) class has the same predecessor and successor tasks as this instance; otherwise, **false**.

## Örnekler

Görev bağlantılarının eşitliğini nasıl kontrol edeceğini gösterir.

```csharp
var project = new Project(DataDir + "GetPredecessorSuccessorTasks.mpp");

var link1 = project.TaskLinks[0];
var link2 = project.TaskLinks[1];

// Görev bağlantılarının eşitliği, ön ve sonraki görevler üzerine temellendirilir.
Console.Write("Link 1 Pred: " + link1.PredTask.ToString());
Console.Write("Link 1 Succ: " + link1.SuccTask.ToString());
Console.Write("Link 2 Pred: " + link2.PredTask.ToString());
Console.Write("Link 2 Succ: " + link2.SuccTask.ToString());
Console.Write("Are task links equal: " + link1.Equals(link2));
```

### Ayrıca Bakınız

* class [TaskLink](../)
* namespace [Aspose.Tasks](../../tasklink/)
* assembly [Aspose.Tasks](../../../)

---

## Equals(object) {#equals_1}

Bu örneğin belirtilen nesneye eşit olup olmadığını gösteren bir değer döndürür.

```csharp
public override bool Equals(object obj)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| obj | Object | Bu örnekle karşılaştırılacak nesne. |

### Dönüş Değeri

**True** if the specified object is a TaskLink that has the same predecessor and successor as this instance; otherwise, **false**.

## Örnekler

Görev bağlantılarının eşitliğini nasıl kontrol edeceğini gösterir.

```csharp
var project = new Project(DataDir + "GetPredecessorSuccessorTasks.mpp");

var link1 = project.TaskLinks[0];
var link2 = project.TaskLinks[1];

// Görev bağlantılarının eşitliği, ön ve sonraki görevler üzerine temellendirilir.
Console.Write("Link 1 Pred: " + link1.PredTask.ToString());
Console.Write("Link 1 Succ: " + link1.SuccTask.ToString());
Console.Write("Link 2 Pred: " + link2.PredTask.ToString());
Console.Write("Link 2 Succ: " + link2.SuccTask.ToString());
Console.Write("Are task links equal: " + link1.Equals(link2));
```

### Ayrıca Bakınız

* class [TaskLink](../)
* namespace [Aspose.Tasks](../../tasklink/)
* assembly [Aspose.Tasks](../../../)


