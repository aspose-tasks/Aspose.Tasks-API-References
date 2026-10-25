---
title: "ExtendedAttributeDefinition.GetHashCode"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Метод ExtendedAttributeDefinition. Возвращает хеш-код для экземпляра класса ExtendedAttributeDefinition."
type: docs
weight: 330
url: /ru/net/aspose.tasks/extendedattributedefinition/gethashcode/
---
## ExtendedAttributeDefinition.GetHashCode method

Возвращает хеш-код для экземпляра класса [`ExtendedAttributeDefinition`](../).

```csharp
public override int GetHashCode()
```

### Возвращаемое значение

хеш-код для этого объекта.

## Примеры

Показывает, как получить хеш-код определения расширенного атрибута.

```csharp
var project = new Project(DataDir + "MultipleOutlineValues2016.mpp");

var attributeDefinition1 = project.ExtendedAttributes.GetById((int)ExtendedAttributeTask.Start3);
var attributeDefinition2 = project.ExtendedAttributes.GetById((int)ExtendedAttributeTask.Duration2);

// хеш-код определения расширенного атрибута равен идентификатору поля.
Console.WriteLine("Extended Attribute Field Id: {0} Hash Code: {1}", attributeDefinition1.FieldId, attributeDefinition1.GetHashCode());
Console.WriteLine("Extended Attribute Field Id: {0} Hash Code: {1}", attributeDefinition2.FieldId, attributeDefinition2.GetHashCode());
```

### См. также

* class [ExtendedAttributeDefinition](../)
* namespace [Aspose.Tasks](../../extendedattributedefinition/)
* assembly [Aspose.Tasks](../../../)


