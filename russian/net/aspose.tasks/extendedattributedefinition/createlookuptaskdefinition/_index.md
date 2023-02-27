---
title: ExtendedAttributeDefinition.CreateLookupTaskDefinition
second_title: Справочник по Aspose.Tasks для .NET API
description: ExtendedAttributeDefinition метод. Фабричный метод который создает расширенное определение атрибута с поиском. Он имеетCalculationType равноLookup и может использоваться только в Заданиях. Необходимо указатьfieldId иalias при вызове этого метода. Тип поля выводится из идентификатора поля.
type: docs
weight: 20
url: /ru/net/aspose.tasks/extendedattributedefinition/createlookuptaskdefinition/
---
## CreateLookupTaskDefinition(ExtendedAttributeTask, string) {#createlookuptaskdefinition_1}

Фабричный метод, который создает расширенное определение атрибута с поиском. Он имеет[`CalculationType`](../calculationtype/) равноLookup и может использоваться только в Заданиях. Необходимо указать*fieldId* и*alias* при вызове этого метода. Тип поля выводится из идентификатора поля.

```csharp
public static ExtendedAttributeDefinition CreateLookupTaskDefinition(ExtendedAttributeTask fieldId, 
    string alias)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| fieldId | ExtendedAttributeTask | Указанный[`ExtendedAttributeTask`](../../extendedattributetask/) идентификатор поля. |
| alias | String | УказанныйString псевдоним. |

### Возвращаемое значение

Созданный экземпляр[`ExtendedAttributeDefinition`](../) класс с указанным*fieldId* и*alias*.

### Примеры

Используйте этот пример, чтобы создать определение пользовательского поля для задачи с поиском, а затем заполнить его текстовыми значениями:

```csharp
var taskTextAttr = ExtendedAttributeDefinition.CreateLookupTaskDefinition(ExtendedAttributeTask.Text27, "My custom field");
taskTextAttr.AddLookupValue(new Value { Id = 1, Val = "Text value 1", Description = "Text value description 1" });
taskTextAttr.AddLookupValue(new Value { Id = 2, Val = "Text value 2", Description = "Text value description 2" });
project.ExtendedAttributes.Add(taskTextAttr);
```

### Смотрите также

* enum [ExtendedAttributeTask](../../extendedattributetask/)
* class [ExtendedAttributeDefinition](../)
* пространство имен [Aspose.Tasks](../../extendedattributedefinition/)
* сборка [Aspose.Tasks](../../../)

---

## CreateLookupTaskDefinition(CustomFieldType, ExtendedAttributeTask, string) {#createlookuptaskdefinition}

Фабричный метод, который создает расширенное определение атрибута с поиском. Он имеет[`CalculationType`](../calculationtype/) равноLookup и может использоваться только в Заданиях. Необходимо указать*customFieldType* ,*fieldId* и*alias* при вызове этого метода.

```csharp
public static ExtendedAttributeDefinition CreateLookupTaskDefinition(
    CustomFieldType customFieldType, ExtendedAttributeTask fieldId, string alias)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| customFieldType | CustomFieldType | Указанный[`CustomFieldType`](../../customfieldtype/) тип. |
| fieldId | ExtendedAttributeTask | Указанный[`ExtendedAttributeTask`](../../extendedattributetask/) идентификатор поля. |
| alias | String | УказанныйString псевдоним. |

### Возвращаемое значение

Созданный экземпляр[`ExtendedAttributeDefinition`](../) класс с указанным*customFieldType* ,*fieldId* и*alias*.

### Примеры

Используйте этот пример, чтобы создать определение пользовательского поля для задачи с поиском, а затем заполнить его текстовыми значениями:

```csharp
var taskTextAttr = ExtendedAttributeDefinition.CreateLookupTaskDefinition(CustomFieldType.Text, ExtendedAttributeTask.Text27, "My custom field");
taskTextAttr.AddLookupValue(new Value { Id = 1, Val = "Text value 1", Description = "Text value description 1" });
taskTextAttr.AddLookupValue(new Value { Id = 2, Val = "Text value 2", Description = "Text value description 2" });
project.ExtendedAttributes.Add(taskTextAttr);
```

### Смотрите также

* enum [CustomFieldType](../../customfieldtype/)
* enum [ExtendedAttributeTask](../../extendedattributetask/)
* class [ExtendedAttributeDefinition](../)
* пространство имен [Aspose.Tasks](../../extendedattributedefinition/)
* сборка [Aspose.Tasks](../../../)


