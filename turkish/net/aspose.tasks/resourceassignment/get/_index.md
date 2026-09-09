---
title: "ResourceAssignment.Get"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "ResourceAssignment yöntemi. Bu kapsayıcıda özelliğin eşlendiği değeri döndürür"
type: docs
weight: 700
url: /tr/net/aspose.tasks/resourceassignment/get/
---
## ResourceAssignment.Get&lt;T&gt; method

Bu kapsayıcıda özelliğin eşlendiği değeri döndürür.

```csharp
public T Get<T>(Key<T, AsnKey> key)
```

| Parametre | Açıklama |
| --- | --- |
| T | eşlenen değerin tipi. |
| key | belirtilen özellik anahtarı. Özellik anahtarını almak için [`Asn`](../../asn/). |

### Dönüş Değeri

özelliğin bu konteynerde eşlendiği değer.

## Örnekler

Bir atama nasıl oluşturulur ve ortak atama özellikleri nasıl alınır/ayarlanır gösterir.

```csharp
var project = new Project(DataDir + "BudgetWorkAndCost.mpp");

var task = project.RootTask.Children.Add("Task");
task.Set(Tsk.Start, new DateTime(2020, 4, 2, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(1));
task.Set(Tsk.Finish, new DateTime(2020, 4, 2, 17, 0, 0));
var resource = project.Resources.Add("Resource");
var resourceAssignment = project.ResourceAssignments.Add(task, resource);
resourceAssignment.Set(Asn.Start, new DateTime(2020, 4, 2, 8, 0, 0));
resourceAssignment.Set(Asn.Work, project.GetWork(1));
resourceAssignment.Set(Asn.Finish, new DateTime(2020, 4, 2, 17, 0, 0));

Console.WriteLine(resourceAssignment.Get(Asn.Start));
Console.WriteLine(resourceAssignment.Get(Asn.Work));
Console.WriteLine(resourceAssignment.Get(Asn.Finish));
```

### Ayrıca Bakınız

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [AsnKey](../../asnkey/)
* class [ResourceAssignment](../)
* namespace [Aspose.Tasks](../../resourceassignment/)
* assembly [Aspose.Tasks](../../../)


