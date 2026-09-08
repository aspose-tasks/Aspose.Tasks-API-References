---
title: "ResourceAssignment.ExtendedAttributes"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Свойство ResourceAssignment. Получает или задает экземпляр класса ExtendedAttributeCollection для этого объекта"
type: docs
weight: 250
url: /ru/net/aspose.tasks/resourceassignment/extendedattributes/
---
## ResourceAssignment.ExtendedAttributes property

Получает или задает экземпляр класса ExtendedAttributeCollection для этого объекта.

```csharp
public ExtendedAttributeCollection ExtendedAttributes { get; set; }
```

## Примечания

Чтение поддерживается только для формата XML.

## Примеры

Показывает, как добавить расширенные атрибуты для назначения.

```csharp
var project = new Project(DataDir + "Blank2010.mpp");

// Назначьте ресурс "1 TRG: Trade Group" задаче "TASK 1", создав объект ResourceAssignment.
var task = project.RootTask.Children.Add("Task");
var resource = project.Resources.Add("Resource");
var assignment = project.ResourceAssignments.Add(task, resource);

// Создайте определение пользовательского атрибута с выпадающим списком.
var definition = ExtendedAttributeDefinition.CreateLookupResourceDefinition(CustomFieldType.Cost, ExtendedAttributeResource.Cost5, "My lookup resource cost");
project.ExtendedAttributes.Add(definition);

var firstValue = new Value { NumericValue = 1500, Description = "Val 1", Id = 1, Val = "1500" };
var secondValue = new Value { NumericValue = 2500, Description = "Val 2", Id = 2 };
definition.AddLookupValue(firstValue);
definition.AddLookupValue(secondValue);

// Это значение можно увидеть в представлении "Resource usage" в MS Project.
var attributeValue = definition.CreateExtendedAttribute(firstValue);
assignment.ExtendedAttributes.Add(attributeValue);

Console.WriteLine("Number of assignment's extended attribute: " + assignment.ExtendedAttributes.Count);
foreach (var attribute in assignment.ExtendedAttributes)
{
    Console.WriteLine("Extended attribute alias: " + attribute.AttributeDefinition.Alias);
}
```

### См. также

* class [ExtendedAttributeCollection](../../extendedattributecollection/)
* class [ResourceAssignment](../)
* namespace [Aspose.Tasks](../../resourceassignment/)
* assembly [Aspose.Tasks](../../../)


