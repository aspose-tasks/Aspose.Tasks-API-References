---
title: "Sınıf ResourceUsageViewFieldCollection"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Aspose.Tasks.ResourceUsageViewFieldCollection sınıfı. ResourceUsageViewField değerlerinin bir koleksiyonunu temsil eder."
type: docs
weight: 1830
url: /tr/net/aspose.tasks/resourceusageviewfieldcollection/
---
## ResourceUsageViewFieldCollection class

[`ResourceUsageViewField`](../resourceusageviewfield/) değerlerinin bir koleksiyonunu temsil eder.

```csharp
public class ResourceUsageViewFieldCollection : IList<ResourceUsageViewField>
```

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| [GetEnumerator](../../aspose.tasks/resourceusageviewfieldcollection/getenumerator/)() | Bu koleksiyon için bir enumerator döndürür. |
| [ToList](../../aspose.tasks/resourceusageviewfieldcollection/tolist/)() | `ResourceUsageViewFieldCollection` sınıfının örneğini, [`ResourceUsageViewField`](../resourceusageviewfield/) sınıfının örneklerini içeren bir listeye dönüştürür. |

## Örnekler

Bir ResourceUsageView örneğinin alan koleksiyonuyla nasıl çalışılacağını gösterir.

```csharp
var project = new Project(DataDir + "ResourceUsageView.mpp");

var view = (ResourceUsageView)project.Views.ToList()[2];
foreach (var field in view.FieldCollection)
{
    Console.WriteLine("Field: " + field);
}

// Koleksiyon bir ResourceUsageViewField listesine dönüştürülebilir.
IList<ResourceUsageViewField> fields = view.FieldCollection.ToList();
foreach (var field in fields)
{
    Console.WriteLine("Field (from the list): " + field);
}
```

### Ayrıca Bakınız

* enum [ResourceUsageViewField](../resourceusageviewfield/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


