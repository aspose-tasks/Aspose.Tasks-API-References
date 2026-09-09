---
title: "Sınıf TaskUsageViewFieldCollection"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Aspose.Tasks.TaskUsageViewFieldCollection sınıfı. TaskUsageViewField değerlerinin bir koleksiyonunu temsil eder"
type: docs
weight: 2500
url: /tr/net/aspose.tasks/taskusageviewfieldcollection/
---
## TaskUsageViewFieldCollection class

[`TaskUsageViewField`](../taskusageviewfield/) değerlerinin bir koleksiyonunu temsil eder.

```csharp
public class TaskUsageViewFieldCollection : IList<TaskUsageViewField>
```

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| [GetEnumerator](../../aspose.tasks/taskusageviewfieldcollection/getenumerator/)() | Bu koleksiyon için bir enumerator döndürür. |
| [ToList](../../aspose.tasks/taskusageviewfieldcollection/tolist/)() | Bu koleksiyondaki tüm öğeleri içeren bir liste döndürür. |

## Örnekler

Bir TaskUsageView örneğinin alan koleksiyonu ile nasıl çalışılacağını gösterir.

```csharp
var project = new Project(DataDir + "TaskUsageView.mpp");

var view = (TaskUsageView)project.Views.ToList()[2];
foreach (var field in view.FieldCollection)
{
    Console.WriteLine("Field: " + field);
}

// Koleksiyon bir TaskUsageViewField listesine dönüştürülebilir
IList<TaskUsageViewField> fields = view.FieldCollection.ToList();
foreach (var field in fields)
{
    Console.WriteLine("Field (from the list): " + field);
}
```

### Ayrıca Bakınız

* enum [TaskUsageViewField](../taskusageviewfield/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


