---
title: ExtendedAttributeDefinition.CreateResourceDefinition
second_title: Справочник по Aspose.Tasks для .NET API
description: ExtendedAttributeDefinition метод. Фабричный метод который создает простое определение расширенного атрибута которое Microsoft Project показывает как Нет. Он имеетCalculationType равноNone и может использоваться только в Ресурсе. Необходимо указатьcustomFieldType fieldId иalias при вызове этого метода.
type: docs
weight: 30
url: /ru/net/aspose.tasks/extendedattributedefinition/createresourcedefinition/
---
## CreateResourceDefinition(CustomFieldType, ExtendedAttributeResource, string) {#createresourcedefinition}

Фабричный метод, который создает простое определение расширенного атрибута, которое Microsoft Project показывает как «Нет». Он имеет[`CalculationType`](../calculationtype/) равноNone и может использоваться только в Ресурсе. Необходимо указать*customFieldType* ,*fieldId* и*alias* при вызове этого метода.

```csharp
public static ExtendedAttributeDefinition CreateResourceDefinition(CustomFieldType customFieldType, 
    ExtendedAttributeResource fieldId, string alias)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| customFieldType | CustomFieldType | Указанный[`CustomFieldType`](../../customfieldtype/) тип. |
| fieldId | ExtendedAttributeResource | Указанный[`ExtendedAttributeResource`](../../extendedattributeresource/) идентификатор поля. |
| alias | String | УказанныйString псевдоним. |

### Возвращаемое значение

Созданный экземпляр[`ExtendedAttributeDefinition`](../) класс с указанным*customFieldType* ,*fieldId* и*alias*.

### Примеры

Используйте этот пример для создания пользовательского определения текстового поля:

```csharp
var resourceTextAttr = ExtendedAttributeDefinition.CreateResourceDefinition(CustomFieldType.Text, ExtendedAttributeResource.Text27, "My custom field");
project.ExtendedAttributes.Add(resourceTextAttr);
```

### Смотрите также

* enum [CustomFieldType](../../customfieldtype/)
* enum [ExtendedAttributeResource](../../extendedattributeresource/)
* class [ExtendedAttributeDefinition](../)
* пространство имен [Aspose.Tasks](../../extendedattributedefinition/)
* сборка [Aspose.Tasks](../../../)

---

## CreateResourceDefinition(ExtendedAttributeResource, string) {#createresourcedefinition_1}

Фабричный метод, который создает простое определение расширенного атрибута, которое Microsoft Project показывает как «Нет». Он имеет[`CalculationType`](../calculationtype/) равноNone и может использоваться только в Ресурсе. Необходимо указать*fieldId* и*alias* при вызове этого метода. Тип поля выводится из идентификатора поля.

```csharp
public static ExtendedAttributeDefinition CreateResourceDefinition(
    ExtendedAttributeResource fieldId, string alias)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| fieldId | ExtendedAttributeResource | Указанный[`ExtendedAttributeResource`](../../extendedattributeresource/) идентификатор поля. |
| alias | String | УказанныйString псевдоним. |

### Возвращаемое значение

Созданный экземпляр[`ExtendedAttributeDefinition`](../) класс с указанным*fieldId* и*alias*.

### Примеры

Используйте этот пример для создания пользовательского определения текстового поля:

```csharp
var resourceTextAttr = ExtendedAttributeDefinition.CreateResourceDefinition(ExtendedAttributeResource.Text27, "My custom field");
project.ExtendedAttributes.Add(resourceTextAttr);
```

### Смотрите также

* enum [ExtendedAttributeResource](../../extendedattributeresource/)
* class [ExtendedAttributeDefinition](../)
* пространство имен [Aspose.Tasks](../../extendedattributedefinition/)
* сборка [Aspose.Tasks](../../../)


