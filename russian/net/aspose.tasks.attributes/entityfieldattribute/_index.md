---
title: "Класс EntityFieldAttribute"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Класс Aspose.Tasks.Attributes.EntityFieldAttribute. Представляет атрибут для свойств сущности"
type: docs
weight: 70
url: /ru/net/aspose.tasks.attributes/entityfieldattribute/
---
## EntityFieldAttribute class

Представляет атрибут для свойств сущности.

```csharp
[AttributeUsage(AttributeTargets.Property)]
public class EntityFieldAttribute : Attribute
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [EntityFieldAttribute](entityfieldattribute/)() | Конструктор по умолчанию. |

## Примечания

Атрибут, используемый только для свойств сущностей [`Task`](../../aspose.tasks/task/), [`Resource`](../../aspose.tasks/resource/), [`Project`](../../aspose.tasks/project/) и [`ResourceAssignment`](../../aspose.tasks/resourceassignment/), и упрощающий их перечисление.

## Примеры

Как перечислять свойства с использованием атрибута **EntityField**:

```csharp
[C#]
var project = new Project("sample.mpp");
foreach (var task in project.SelectAllChildTasks())
{
    Console.WriteLine("Task:");
    foreach (var propInfo in typeof(Task).GetProperties().Where(propInfo => propInfo.GetCustomAttribute{Attributes.EntityFieldAttribute}() != null))
    {
        Console.WriteLine(string.Format("{0}: {1}", propInfo.Name, propInfo.GetValue(task)));
    }
}
```

### См. также

* namespace [Aspose.Tasks.Attributes](../../aspose.tasks.attributes/)
* assembly [Aspose.Tasks](../../)


