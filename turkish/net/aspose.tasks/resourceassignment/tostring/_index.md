---
title: "ResourceAssignment.ToString"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "ResourceAssignment yöntemi. ResourceAssignment sınıfının örneğinin kısa dize temsilini döndürür. Temsilin kesin ayrıntıları belirtilmemiştir ve değişebilir"
type: docs
weight: 790
url: /tr/net/aspose.tasks/resourceassignment/tostring/
---
## ResourceAssignment.ToString method

[`ResourceAssignment`](../) sınıfının örneğinin kısa dize temsilini döndürür. Temsilin kesin ayrıntıları belirtilmemiştir ve değişebilir.

```csharp
public override string ToString()
```

### Dönüş Değeri

atanma nesnesini temsil eden kısa dize.

## Örnekler

ortak atama bilgilerini nasıl yazdıracağınızı gösterir.

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

* class [ResourceAssignment](../)
* namespace [Aspose.Tasks](../../resourceassignment/)
* assembly [Aspose.Tasks](../../../)


