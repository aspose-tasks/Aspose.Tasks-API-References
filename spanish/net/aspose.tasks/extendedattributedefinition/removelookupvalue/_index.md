---
title: "ExtendedAttributeDefinition.RemoveLookupValue"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Método ExtendedAttributeDefinition. Elimina un valor de la lista de búsqueda interna. Esta es una forma preferible de manipular la ValueList"
type: docs
weight: 340
url: /es/net/aspose.tasks/extendedattributedefinition/removelookupvalue/
---
## ExtendedAttributeDefinition.RemoveLookupValue method

Elimina un valor de la lista de búsqueda interna. Esta es una forma preferible de manipular la [`ValueList`](../valuelist/).

```csharp
public void RemoveLookupValue(Value value)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | Valor | Valor a eliminar de la búsqueda. |

## Observaciones

Este método funciona solo para instancias de [`ExtendedAttributeDefinition`](../) que tengan [`CalculationType`](../calculationtype/) igual a Lookup.

## Ejemplos

Muestra cómo agregar atributos extendidos con búsquedas para asignaciones.

```csharp
var project = new Project(DataDir + "Blank2010.mpp");

// Asigne el recurso "1 TRG: Trade Group" a la "TASK 1" creando un objeto ResourceAssignment.
var resource = project.Resources.GetById(1);
var task = project.RootTask.Children.GetById(1);
var assignment = project.ResourceAssignments.Add(task, resource);

// Cree una definición de atributo personalizado con búsqueda.
var resExtendedAttributeDefinition = ExtendedAttributeDefinition.CreateLookupResourceDefinition(
    CustomFieldType.Cost,
    ExtendedAttributeResource.Cost5,
    "My lookup resource cost");
project.ExtendedAttributes.Add(resExtendedAttributeDefinition);

var firstValue = new Value { NumericValue = 1500, Description = "Val 1", Id = 1, Val = "1500" };
var secondValue = new Value { NumericValue = 2500, Description = "Val 2", Id = 2 };
resExtendedAttributeDefinition.AddLookupValue(firstValue);
resExtendedAttributeDefinition.AddLookupValue(secondValue);

// Este valor se puede ver en la vista "Resource usage" de MS Project.
var attributeValue = resExtendedAttributeDefinition.CreateExtendedAttribute(firstValue);
assignment.ExtendedAttributes.Add(attributeValue);

// Cree una definición de atributo personalizado con búsqueda.
var taskCostAttr = ExtendedAttributeDefinition.CreateLookupTaskDefinition(CustomFieldType.Cost, ExtendedAttributeTask.Cost4, "My lookup task cost");
project.ExtendedAttributes.Add(taskCostAttr);
var taskFirstValue = new Value { NumericValue = 18, Description = "Task val 1", Id = 3, Val = "18" };
var resSecondValue = new Value { NumericValue = 30, Description = "Task val 2", Id = 4 };
var taskWrongValue = new Value { NumericValue = 99, Description = "Task val Wrong", Id = 5, Val = "18" };

taskCostAttr.AddLookupValue(taskFirstValue);
resExtendedAttributeDefinition.AddLookupValue(resSecondValue);

// Este valor se puede ver en la vista "Task usage" de MS Project.
assignment.ExtendedAttributes.Add(taskCostAttr.CreateExtendedAttribute(taskFirstValue));

// Los valores incorrectos pueden eliminarse más tarde.
taskCostAttr.RemoveLookupValue(taskWrongValue);

// Trabajando con el proyecto...
```

### Ver también

* class [Value](../../value/)
* class [ExtendedAttributeDefinition](../)
* namespace [Aspose.Tasks](../../extendedattributedefinition/)
* assembly [Aspose.Tasks](../../../)


