---
title: "TaskUsageViewFieldCollection.ToList"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "TaskUsageViewFieldCollection yöntemi. Bu koleksiyondaki tüm öğeleri içeren bir liste döndürür."
type: docs
weight: 20
url: /tr/net/aspose.tasks/taskusageviewfieldcollection/tolist/
---
## TaskUsageViewFieldCollection.ToList method

Bu koleksiyondaki tüm öğeleri içeren bir liste döndürür.

```csharp
public IList<TaskUsageViewField> ToList()
```

### Dönüş Değeri

Bu koleksiyondaki tüm öğeleri içeren bir liste döndürür.

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

* enum [TaskUsageViewField](../../taskusageviewfield/)
* class [TaskUsageViewFieldCollection](../)
* namespace [Aspose.Tasks](../../taskusageviewfieldcollection/)
* assembly [Aspose.Tasks](../../../)


