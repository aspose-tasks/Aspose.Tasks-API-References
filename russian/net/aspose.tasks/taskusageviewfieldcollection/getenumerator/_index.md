---
title: "TaskUsageViewFieldCollection.GetEnumerator"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "TaskUsageViewFieldCollection метод. Возвращает перечислитель для этой коллекции"
type: docs
weight: 10
url: /ru/net/aspose.tasks/taskusageviewfieldcollection/getenumerator/
---
## TaskUsageViewFieldCollection.GetEnumerator method

Возвращает перечислитель для этой коллекции.

```csharp
public IEnumerator<TaskUsageViewField> GetEnumerator()
```

### Возвращаемое значение

перечислитель для этой коллекции.

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


