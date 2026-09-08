---
title: "ResourceUsageViewFieldCollection.ToList"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Метод ResourceUsageViewFieldCollection. Преобразует экземпляр класса ResourceUsageViewFieldCollection в список, содержащий экземпляры класса ResourceUsageViewField"
type: docs
weight: 20
url: /ru/net/aspose.tasks/resourceusageviewfieldcollection/tolist/
---
## ResourceUsageViewFieldCollection.ToList method

Преобразует экземпляр класса [`ResourceUsageViewFieldCollection`](../) в список, содержащий экземпляры класса [`ResourceUsageViewField`](../../resourceusageviewfield/).

```csharp
public IList<ResourceUsageViewField> ToList()
```

### Возвращаемое значение

Экземпляр класса [`ResourceUsageViewFieldCollection`](../), преобразованный в список, содержащий экземпляры класса [`ResourceUsageViewField`](../../resourceusageviewfield/).

## Примеры

Показывает, как работать с коллекцией полей экземпляра ResourceUsageView.

```csharp
var project = new Project(DataDir + "ResourceUsageView.mpp");

var view = (ResourceUsageView)project.Views.ToList()[2];
foreach (var field in view.FieldCollection)
{
    Console.WriteLine("Field: " + field);
}

// Можно преобразовать коллекцию в список ResourceUsageViewField.
IList<ResourceUsageViewField> fields = view.FieldCollection.ToList();
foreach (var field in fields)
{
    Console.WriteLine("Field (from the list): " + field);
}
```

### См. также

* enum [ResourceUsageViewField](../../resourceusageviewfield/)
* class [ResourceUsageViewFieldCollection](../)
* namespace [Aspose.Tasks](../../resourceusageviewfieldcollection/)
* assembly [Aspose.Tasks](../../../)


