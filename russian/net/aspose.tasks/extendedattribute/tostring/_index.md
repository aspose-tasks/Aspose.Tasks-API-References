---
title: "ExtendedAttribute.ToString"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Метод ExtendedAttribute. Возвращает короткое строковое представление расширенного атрибута"
type: docs
weight: 110
url: /ru/net/aspose.tasks/extendedattribute/tostring/
---
## ExtendedAttribute.ToString method

Возвращает краткое строковое представление расширенного атрибута.

```csharp
public override string ToString()
```

### Возвращаемое значение

Строковое представление расширенного атрибута.

## Примеры

Показывает, как читать расширенные атрибуты.

```csharp
var project = new Project(DataDir + "ReadTaskExtendedAttributes.mpp");

// Чтение расширенных атрибутов для задач
foreach (var task in project.RootTask.Children)
{
    foreach (var attribute in task.ExtendedAttributes)
    {
        // читать общую информацию о расширенном атрибуте
        Console.WriteLine("Extended Attribute: " + attribute.ToString());
    }
}
```

### См. также

* class [ExtendedAttribute](../)
* namespace [Aspose.Tasks](../../extendedattribute/)
* assembly [Aspose.Tasks](../../../)


