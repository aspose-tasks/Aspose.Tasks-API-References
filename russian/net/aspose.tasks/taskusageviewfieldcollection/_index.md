---
title: "Класс TaskUsageViewFieldCollection"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Класс Aspose.Tasks.TaskUsageViewFieldCollection. Представляет коллекцию значений TaskUsageViewField."
type: docs
weight: 2500
url: /ru/net/aspose.tasks/taskusageviewfieldcollection/
---
## TaskUsageViewFieldCollection class

Представляет коллекцию значений [`TaskUsageViewField`](../taskusageviewfield/).

```csharp
public class TaskUsageViewFieldCollection : IList<TaskUsageViewField>
```

## Методы

| Имя | Описание |
| --- | --- |
| [GetEnumerator](../../aspose.tasks/taskusageviewfieldcollection/getenumerator/)() | Возвращает перечислитель для этой коллекции. |
| [ToList](../../aspose.tasks/taskusageviewfieldcollection/tolist/)() | Возвращает список, содержащий все элементы этой коллекции. |

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

* enum [TaskUsageViewField](../taskusageviewfield/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


