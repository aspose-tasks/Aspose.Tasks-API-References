---
title: ExtendedAttributeDefinition.CreateTaskDefinition
second_title: Справочник по Aspose.Tasks для .NET API
description: ExtendedAttributeDefinition метод. Фабричный метод который создает простое определение расширенного атрибута которое Microsoft Project показывает как Нет. Он имеетCalculationType равноNone и может использоваться только в Заданиях. Необходимо указатьcustomFieldType fieldId иalias при вызове этого метода.
type: docs
weight: 40
url: /ru/net/aspose.tasks/extendedattributedefinition/createtaskdefinition/
---
## CreateTaskDefinition(CustomFieldType, ExtendedAttributeTask, string) {#createtaskdefinition}

Фабричный метод, который создает простое определение расширенного атрибута, которое Microsoft Project показывает как «Нет». Он имеет[`CalculationType`](../calculationtype/) равноNone и может использоваться только в Заданиях. Необходимо указать*customFieldType* ,*fieldId* и*alias* при вызове этого метода.

```csharp
public static ExtendedAttributeDefinition CreateTaskDefinition(CustomFieldType customFieldType, 
    ExtendedAttributeTask fieldId, string alias)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| customFieldType | CustomFieldType | Указанный[`CustomFieldType`](../../customfieldtype/) тип. |
| fieldId | ExtendedAttributeTask | Указанный[`ExtendedAttributeTask`](../../extendedattributetask/) идентификатор поля. |
| alias | String | УказанныйString псевдоним. |

### Возвращаемое значение

Созданный экземпляр[`ExtendedAttributeDefinition`](../) класс с указанным*customFieldType* ,*fieldId* и*alias*.

### Примеры

Используйте этот пример для создания пользовательского определения текстового поля:

```csharp
var taskTextAttr = ExtendedAttributeDefinition.CreateTaskDefinition(CustomFieldType.Text, ExtendedAttributeTask.Text27, "My custom field");
project.ExtendedAttributes.Add(taskTextAttr);
```

### Смотрите также

* enum [CustomFieldType](../../customfieldtype/)
* enum [ExtendedAttributeTask](../../extendedattributetask/)
* class [ExtendedAttributeDefinition](../)
* пространство имен [Aspose.Tasks](../../extendedattributedefinition/)
* сборка [Aspose.Tasks](../../../)

---

## CreateTaskDefinition(ExtendedAttributeTask, string) {#createtaskdefinition_1}

Фабричный метод, который создает простое определение расширенного атрибута, которое Microsoft Project показывает как «Нет». Он имеет[`CalculationType`](../calculationtype/) равноNone и может использоваться только в Заданиях. Необходимо указать*fieldId* и*alias* при вызове этого метода. Тип поля выводится из идентификатора поля.

```csharp
public static ExtendedAttributeDefinition CreateTaskDefinition(ExtendedAttributeTask fieldId, 
    string alias)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| fieldId | ExtendedAttributeTask | Указанный[`ExtendedAttributeTask`](../../extendedattributetask/) идентификатор поля. |
| alias | String | УказанныйString псевдоним. |

### Возвращаемое значение

Созданный экземпляр[`ExtendedAttributeDefinition`](../) класс с указанным*fieldId* и*alias*.

### Примеры

Используйте этот пример для создания пользовательского определения текстового поля:

```csharp
var taskTextAttr = ExtendedAttributeDefinition.CreateTaskDefinition(ExtendedAttributeTask.Text27, "My custom field");
project.ExtendedAttributes.Add(taskTextAttr);
```

### Смотрите также

* enum [ExtendedAttributeTask](../../extendedattributetask/)
* class [ExtendedAttributeDefinition](../)
* пространство имен [Aspose.Tasks](../../extendedattributedefinition/)
* сборка [Aspose.Tasks](../../../)


