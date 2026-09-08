---
title: "Resource.ExtendedAttributes"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Свойство Resource. Получает значения расширенного атрибута"
type: docs
weight: 320
url: /ru/net/aspose.tasks/resource/extendedattributes/
---
## Resource.ExtendedAttributes property

Получает значения расширенного атрибута.

```csharp
public ExtendedAttributeCollection ExtendedAttributes { get; }
```

## Примечания

Необходимо два элемента данных — указатель на таблицу расширенных атрибутов, который задаётся либо уникальным идентификатором, либо идентификатором поля, и значение, которое задаётся либо непосредственно значением, либо указателем на список значений.

## Примеры

Показывает, как добавить расширенные атрибуты ресурса.

```csharp
var project = new Project(DataDir + "ResourceExtendedAttributes.mpp");

// Определить расширенный атрибут
var definition = project.ExtendedAttributes.GetById((int)ExtendedAttributeTask.Number1);
if (definition == null)
{
    definition = ExtendedAttributeDefinition.CreateResourceDefinition(ExtendedAttributeResource.Number1, "Age");
    project.ExtendedAttributes.Add(definition);
}

// Создать расширенный атрибут и установить его значение
var attribute = definition.CreateExtendedAttribute();
attribute.NumericValue = 30.5345m;

// Добавить новый ресурс и его расширенный атрибут   
var resource = project.Resources.Add("R1");
resource.ExtendedAttributes.Add(attribute);

project.Save(OutDir + "ResourceExtendedAttributes_out.mpp", SaveFileFormat.Mpp);
```

### См. также

* class [ExtendedAttributeCollection](../../extendedattributecollection/)
* class [Resource](../)
* namespace [Aspose.Tasks](../../resource/)
* assembly [Aspose.Tasks](../../../)


