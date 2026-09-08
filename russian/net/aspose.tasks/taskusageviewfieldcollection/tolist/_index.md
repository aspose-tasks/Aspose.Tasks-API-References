---
title: "TaskUsageViewFieldCollection.ToList"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "TaskUsageViewFieldCollection метод. Возвращает список, содержащий все элементы этой коллекции"
type: docs
weight: 20
url: /ru/net/aspose.tasks/taskusageviewfieldcollection/tolist/
---
## TaskUsageViewFieldCollection.ToList method

Возвращает список, содержащий все элементы этой коллекции.

```csharp
public IList<TaskUsageViewField> ToList()
```

### Возвращаемое значение

возвращает список, содержащий все элементы этой коллекции.

## Примеры

Показывает, как работать с коллекцией полей экземпляра TaskUsageView.

```csharp
var project = new Project(DataDir + "TaskUsageView.mpp");

var view = (TaskUsageView)project.Views.ToList()[2];
foreach (var field in view.FieldCollection)
{
    Console.WriteLine("Field: " + field);
}

// Можно преобразовать коллекцию в список TaskUsageViewField.
IList<TaskUsageViewField> fields = view.FieldCollection.ToList();
foreach (var field in fields)
{
    Console.WriteLine("Field (from the list): " + field);
}
```

### См. также

* enum [TaskUsageViewField](../../taskusageviewfield/)
* class [TaskUsageViewFieldCollection](../)
* namespace [Aspose.Tasks](../../taskusageviewfieldcollection/)
* assembly [Aspose.Tasks](../../../)


