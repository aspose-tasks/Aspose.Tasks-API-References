---
title: "ExtendedAttributeDefinition.Equals"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Метод ExtendedAttributeDefinition. Возвращает флаг, указывающий, равен ли этот экземпляр указанному объекту"
type: docs
weight: 320
url: /ru/net/aspose.tasks/extendedattributedefinition/equals/
---
## ExtendedAttributeDefinition.Equals method

Возвращает флаг, указывающий, равен ли этот экземпляр указанному объекту.

```csharp
public override bool Equals(object obj)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| obj | Объект | указанный объект для сравнения с этим экземпляром. |

### Возвращаемое значение

флаг, указывающий, равен ли этот экземпляр указанному объекту.

## Примеры

Показывает, как проверить равенство определения расширенного атрибута.

```csharp
var project = new Project(DataDir + "MultipleOutlineValues2016.mpp");

var attributeDefinition1 = project.ExtendedAttributes.GetById((int)ExtendedAttributeTask.Start3);
var attributeDefinition2 = project.ExtendedAttributes.GetById((int)ExtendedAttributeTask.Duration2);

// равенство календарей проверяется по идентификаторам полей определения атрибута.
Console.WriteLine("ExtendedAttribute 1 Field Id: " + attributeDefinition1.FieldId);
Console.WriteLine("ExtendedAttribute 2 Field Id: " + attributeDefinition2.FieldId);
Console.WriteLine("Are extended attributes equal: " + attributeDefinition1.Equals(attributeDefinition2));
```

### См. также

* class [ExtendedAttributeDefinition](../)
* namespace [Aspose.Tasks](../../extendedattributedefinition/)
* assembly [Aspose.Tasks](../../../)


