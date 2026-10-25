---
title: "Класс ResourceUsageViewFieldCollection"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Класс Aspose.Tasks.ResourceUsageViewFieldCollection. Представляет коллекцию значений ResourceUsageViewField."
type: docs
weight: 1830
url: /ru/net/aspose.tasks/resourceusageviewfieldcollection/
---
## ResourceUsageViewFieldCollection class

Представляет коллекцию значений [`ResourceUsageViewField`](../resourceusageviewfield/).

```csharp
public class ResourceUsageViewFieldCollection : IList<ResourceUsageViewField>
```

## Методы

| Имя | Описание |
| --- | --- |
| [GetEnumerator](../../aspose.tasks/resourceusageviewfieldcollection/getenumerator/)() | Возвращает перечислитель для этой коллекции. |
| [ToList](../../aspose.tasks/resourceusageviewfieldcollection/tolist/)() | Преобразует экземпляр класса `ResourceUsageViewFieldCollection` в список, содержащий экземпляры класса [`ResourceUsageViewField`](../resourceusageviewfield/). |

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

* enum [ResourceUsageViewField](../resourceusageviewfield/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


