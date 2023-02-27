---
title: ExtendedAttributeDefinition.CreateLookupResourceDefinition
second_title: Справочник по Aspose.Tasks для .NET API
description: ExtendedAttributeDefinition метод. Фабричный метод который создает расширенное определение атрибута с поиском. Он имеетCalculationType равноLookup и может использоваться только в Ресурсах. Необходимо указатьfieldId иalias при вызове этого метода. Тип поля выводится из идентификатора поля.
type: docs
weight: 10
url: /ru/net/aspose.tasks/extendedattributedefinition/createlookupresourcedefinition/
---
## CreateLookupResourceDefinition(ExtendedAttributeResource, string) {#createlookupresourcedefinition_1}

Фабричный метод, который создает расширенное определение атрибута с поиском. Он имеет[`CalculationType`](../calculationtype/) равноLookup и может использоваться только в Ресурсах. Необходимо указать*fieldId* и*alias* при вызове этого метода. Тип поля выводится из идентификатора поля.

```csharp
public static ExtendedAttributeDefinition CreateLookupResourceDefinition(
    ExtendedAttributeResource fieldId, string alias)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| fieldId | ExtendedAttributeResource | Указанный[`ExtendedAttributeResource`](../../extendedattributeresource/) идентификатор поля. |
| alias | String | УказанныйString псевдоним. |

### Возвращаемое значение

Созданный экземпляр[`ExtendedAttributeDefinition`](../) класс с указанным*fieldId* и*alias*.

### Примеры

Используйте этот пример, чтобы создать определение пользовательского поля для ресурса с поиском, а затем заполнить его текстовыми значениями:

```csharp
var resourceTextAttr = ExtendedAttributeDefinition.CreateLookupResourceDefinition(ExtendedAttributeResource.Text27, "My custom field");
resourceTextAttr.AddLookupValue(new Value { Id = 1, Val = "Text value 1", Description = "Text value description 1" });
resourceTextAttr.AddLookupValue(new Value { Id = 2, Val = "Text value 2", Description = "Text value description 2" });
project.ExtendedAttributes.Add(resourceTextAttr);
```

### Смотрите также

* enum [ExtendedAttributeResource](../../extendedattributeresource/)
* class [ExtendedAttributeDefinition](../)
* пространство имен [Aspose.Tasks](../../extendedattributedefinition/)
* сборка [Aspose.Tasks](../../../)

---

## CreateLookupResourceDefinition(CustomFieldType, ExtendedAttributeResource, string) {#createlookupresourcedefinition}

Фабричный метод, который создает расширенное определение атрибута с поиском. Он имеет[`CalculationType`](../calculationtype/) равноLookup и может использоваться только в Ресурсах. Необходимо указать*customFieldType* ,*fieldId* и*alias* при вызове этого метода.

```csharp
public static ExtendedAttributeDefinition CreateLookupResourceDefinition(
    CustomFieldType customFieldType, ExtendedAttributeResource fieldId, string alias)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| customFieldType | CustomFieldType | Указанный[`CustomFieldType`](../../customfieldtype/) тип. |
| fieldId | ExtendedAttributeResource | Указанный[`ExtendedAttributeResource`](../../extendedattributeresource/) идентификатор поля. |
| alias | String | УказанныйString псевдоним. |

### Возвращаемое значение

Созданный экземпляр[`ExtendedAttributeDefinition`](../) класс с указанным*customFieldType* ,*fieldId* и*alias*.

### Примеры

Используйте этот пример, чтобы создать определение пользовательского поля для ресурса с поиском, а затем заполнить его текстовыми значениями:

```csharp
var resourceTextAttr = ExtendedAttributeDefinition.CreateLookupResourceDefinition(CustomFieldType.Text, ExtendedAttributeResource.Text27, "My custom field");
resourceTextAttr.AddLookupValue(new Value { Id = 1, Val = "Text value 1", Description = "Text value description 1" });
resourceTextAttr.AddLookupValue(new Value { Id = 2, Val = "Text value 2", Description = "Text value description 2" });
project.ExtendedAttributes.Add(resourceTextAttr);
```

### Смотрите также

* enum [CustomFieldType](../../customfieldtype/)
* enum [ExtendedAttributeResource](../../extendedattributeresource/)
* class [ExtendedAttributeDefinition](../)
* пространство имен [Aspose.Tasks](../../extendedattributedefinition/)
* сборка [Aspose.Tasks](../../../)


