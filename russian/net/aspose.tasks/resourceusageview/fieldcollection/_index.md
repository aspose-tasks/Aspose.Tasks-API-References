---
title: "ResourceUsageView.FieldCollection"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Свойство ResourceUsageView. Получает объект ResourceUsageViewFieldCollection данного ResourceUsageView."
type: docs
weight: 10
url: /ru/net/aspose.tasks/resourceusageview/fieldcollection/
---
## ResourceUsageView.FieldCollection property

Получает объект [`ResourceUsageViewFieldCollection`](../../resourceusageviewfieldcollection/) данного ResourceUsageView.

```csharp
public ResourceUsageViewFieldCollection FieldCollection { get; }
```

## Примеры

Показывает, как читать поля представления использования ресурсов.

```csharp
var project = new Project(DataDir + "ResourceUsageView.mpp");

var view = (ResourceUsageView)project.Views.ToList()[2];
foreach (var field in view.FieldCollection)
{
    Console.WriteLine("Field: " + field);
}
```

### См. также

* class [ResourceUsageViewFieldCollection](../../resourceusageviewfieldcollection/)
* class [ResourceUsageView](../)
* namespace [Aspose.Tasks](../../resourceusageview/)
* assembly [Aspose.Tasks](../../../)


