---
title: "ResourceUsageViewFieldCollection.ToList"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "ResourceUsageViewFieldCollection yöntemi. ResourceUsageViewFieldCollection sınıfının örneğini, ResourceUsageViewField sınıfının örneklerini içeren bir listeye dönüştürür"
type: docs
weight: 20
url: /tr/net/aspose.tasks/resourceusageviewfieldcollection/tolist/
---
## ResourceUsageViewFieldCollection.ToList method

[`ResourceUsageViewFieldCollection`](../) sınıfının örneğini, [`ResourceUsageViewField`](../../resourceusageviewfield/) sınıfının örneklerini içeren bir listeye dönüştürür.

```csharp
public IList<ResourceUsageViewField> ToList()
```

### Dönüş Değeri

[`ResourceUsageViewFieldCollection`](../) sınıfının örneği, [`ResourceUsageViewField`](../../resourceusageviewfield/) sınıfının örneklerini içeren bir listeye dönüştürülür.

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

* enum [ResourceUsageViewField](../../resourceusageviewfield/)
* class [ResourceUsageViewFieldCollection](../)
* namespace [Aspose.Tasks](../../resourceusageviewfieldcollection/)
* assembly [Aspose.Tasks](../../../)


