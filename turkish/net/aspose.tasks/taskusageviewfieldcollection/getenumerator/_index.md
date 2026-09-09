---
title: "TaskUsageViewFieldCollection.GetEnumerator"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "TaskUsageViewFieldCollection yöntemi. Bu koleksiyon için bir yineleyici döndürür."
type: docs
weight: 10
url: /tr/net/aspose.tasks/taskusageviewfieldcollection/getenumerator/
---
## TaskUsageViewFieldCollection.GetEnumerator method

Bu koleksiyon için bir enumerator döndürür.

```csharp
public IEnumerator<TaskUsageViewField> GetEnumerator()
```

### Dönüş Değeri

bu koleksiyon için bir yineleyici.

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


