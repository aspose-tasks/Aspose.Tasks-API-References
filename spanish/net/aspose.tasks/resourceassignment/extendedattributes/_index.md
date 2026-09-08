---
title: "ResourceAssignment.ExtendedAttributes"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "ResourceAssignment propiedad. Obtiene o establece una instancia de la clase ExtendedAttributeCollection para este objeto"
type: docs
weight: 250
url: /es/net/aspose.tasks/resourceassignment/extendedattributes/
---
## ResourceAssignment.ExtendedAttributes property

Obtiene o establece una instancia de la clase ExtendedAttributeCollection para este objeto.

```csharp
public ExtendedAttributeCollection ExtendedAttributes { get; set; }
```

## Observaciones

Lectura soportada solo para formato XML.

## Ejemplos

Muestra cómo agregar atributos extendidos para una asignación.

```csharp
var project = new Project(DataDir + "Blank2010.mpp");

// Asigne el recurso "1 TRG: Trade Group" a la "TASK 1" creando un objeto ResourceAssignment.
var task = project.RootTask.Children.Add("Task");
var resource = project.Resources.Add("Resource");
var assignment = project.ResourceAssignments.Add(task, resource);

// Cree una definición de atributo personalizado con búsqueda.
var definition = ExtendedAttributeDefinition.CreateLookupResourceDefinition(CustomFieldType.Cost, ExtendedAttributeResource.Cost5, "My lookup resource cost");
project.ExtendedAttributes.Add(definition);

var firstValue = new Value { NumericValue = 1500, Description = "Val 1", Id = 1, Val = "1500" };
var secondValue = new Value { NumericValue = 2500, Description = "Val 2", Id = 2 };
definition.AddLookupValue(firstValue);
definition.AddLookupValue(secondValue);

// Este valor se puede ver en la vista "Resource usage" de MS Project.
var attributeValue = definition.CreateExtendedAttribute(firstValue);
assignment.ExtendedAttributes.Add(attributeValue);

Console.WriteLine("Number of assignment's extended attribute: " + assignment.ExtendedAttributes.Count);
foreach (var attribute in assignment.ExtendedAttributes)
{
    Console.WriteLine("Extended attribute alias: " + attribute.AttributeDefinition.Alias);
}
```

### Ver también

* class [ExtendedAttributeCollection](../../extendedattributecollection/)
* class [ResourceAssignment](../)
* namespace [Aspose.Tasks](../../resourceassignment/)
* assembly [Aspose.Tasks](../../../)


