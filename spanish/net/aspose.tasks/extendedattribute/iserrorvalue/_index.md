---
title: "ExtendedAttribute.IsErrorValue"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Propiedad ExtendedAttribute. Obtiene si el cálculo del valor de los atributos extendidos resultó en un error"
type: docs
weight: 60
url: /es/net/aspose.tasks/extendedattribute/iserrorvalue/
---
## ExtendedAttribute.IsErrorValue property

Obtiene si el cálculo del valor del atributo extendido resultó en un error.

```csharp
public bool IsErrorValue { get; }
```

## Ejemplos

Muestra cómo agregar un campo personalizado cuyo valor se calcula usando la fórmula especificada por el usuario.

```csharp
var project = new Project();

// crear nueva definición de atributo extendido de tarea
var attribute = ExtendedAttributeDefinition.CreateTaskDefinition(CustomFieldType.Cost, ExtendedAttributeTask.Cost1, "Cost ratio");

// Agregar una fórmula al atributo.
attribute.Formula = "[Cost] / [Actual Cost]";

project.ExtendedAttributes.Add(attribute);

var task = project.RootTask.Children.Add("Task");

// Crear atributo extendido
var extendedAttribute = attribute.CreateExtendedAttribute();
task.ExtendedAttributes.Add(extendedAttribute);

// Establecemos la Formula para el atributo extendido, por lo que es de solo lectura (el valor se calcula usando la fórmula).
// La salida es "El valor es de solo lectura"
Console.WriteLine(extendedAttribute.ValueReadOnly ? "Value is read only" : "Value is not read only");

// Puedes intentar establecer el valor de un campo de solo lectura, pero no tendrá efecto.
extendedAttribute.NumericValue = -1000000M;

Console.WriteLine("Cost is {0}, Actual Cost is {1}, Custom attribute's value is {2}",
    task.Get(Tsk.Cost),
    task.Get(Tsk.ActualCost),
    extendedAttribute.IsErrorValue ? "#Error" : extendedAttribute.NumericValue.ToString());

task.Set(Tsk.Cost, 100m);
task.Set(Tsk.ActualCost, 120m);

Console.WriteLine("Cost is {0}, Actual Cost is {1}, Custom attribute's value is {2}",
    task.Get(Tsk.Cost), 
    task.Get(Tsk.ActualCost),
    extendedAttribute.IsErrorValue ? "#Error" : extendedAttribute.NumericValue.ToString());
```

### Ver también

* class [ExtendedAttribute](../)
* namespace [Aspose.Tasks](../../extendedattribute/)
* assembly [Aspose.Tasks](../../../)


