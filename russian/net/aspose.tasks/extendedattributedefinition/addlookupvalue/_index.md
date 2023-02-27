---
title: ExtendedAttributeDefinition.AddLookupValue
second_title: Справочник по Aspose.Tasks для .NET API
description: ExtendedAttributeDefinition метод. Добавляет значение во внутренний список поиска. Это предпочтительный способ для манипуляций сValueList .
type: docs
weight: 290
url: /ru/net/aspose.tasks/extendedattributedefinition/addlookupvalue/
---
## ExtendedAttributeDefinition.AddLookupValue method

Добавляет значение во внутренний список поиска. Это предпочтительный способ для манипуляций с[`ValueList`](../valuelist/) .

```csharp
public void AddLookupValue(Value value)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| value | Value | Значение для добавления в поиск. |

### Примечания

Этот метод работает только для[`ExtendedAttributeDefinition`](../) instances , которые имеют[`CalculationType`](../calculationtype/) равноLookup .

### Примеры

Используйте этот код, чтобы добавить новое значение в список поиска:

```csharp
taskTextAttr.AddLookupValue(new Value { Id = 1, Val = "Text value 1", Description = "Text value description 1" });
```

### Смотрите также

* class [Value](../../value/)
* class [ExtendedAttributeDefinition](../)
* пространство имен [Aspose.Tasks](../../extendedattributedefinition/)
* сборка [Aspose.Tasks](../../../)


