---
title: Class EntityFieldAttribute
second_title: Справочник по Aspose.Tasks для .NET API
description: Aspose.Tasks.Attributes.EntityFieldAttribute сорт. Представляет атрибут для свойств объекта.
type: docs
weight: 70
url: /ru/net/aspose.tasks.attributes/entityfieldattribute/
---
## EntityFieldAttribute class

Представляет атрибут для свойств объекта.

```csharp
[AttributeUsage(AttributeTargets.Property)]
public class EntityFieldAttribute : Attribute
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [EntityFieldAttribute](entityfieldattribute/)() | Конструктор по умолчанию. |

### Примечания

Атрибут, используемый для[`Task`](../../aspose.tasks/task/) ,[`Resource`](../../aspose.tasks/resource/) ,[`Project`](../../aspose.tasks/project/) и[`ResourceAssignment`](../../aspose.tasks/resourceassignment/) только свойства объекта и упрощает его перечисление.

### Примеры

Как перечислить свойства с помощью **EntityField** атрибут:

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

### Смотрите также

* пространство имен [Aspose.Tasks.Attributes](../../aspose.tasks.attributes/)
* сборка [Aspose.Tasks](../../)


