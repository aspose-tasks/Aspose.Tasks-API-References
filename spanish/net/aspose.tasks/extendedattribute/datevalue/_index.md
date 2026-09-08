---
title: "ExtendedAttribute.DateValue"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Propiedad ExtendedAttribute. Obtiene o establece un valor para atributos con tipos de fecha Date Start Finish"
type: docs
weight: 20
url: /es/net/aspose.tasks/extendedattribute/datevalue/
---
## ExtendedAttribute.DateValue property

Obtiene o establece un valor para atributos con tipos de fecha (Date, Start, Finish).

```csharp
public DateTime DateValue { get; set; }
```

### Excepciones

| excepción | condición |
| --- | --- |
| InvalidOperationException | Se lanza si la propiedad [`AttributeDefinition`](../attributedefinition/) no está inicializada o el atributo actual no es un atributo de fecha. |

## Ejemplos

Muestra cómo cambiar la definición del atributo del atributo extendido.

```csharp
var project = new Project();

// crear nueva definición de atributo extendido de tarea
var definition = ExtendedAttributeDefinition.CreateTaskDefinition(CustomFieldType.Cost, ExtendedAttributeTask.Cost1, string.Empty);

// Agregar una fórmula al atributo.
definition.Alias = "Difference between Cost and Actual Cost";
definition.Formula = "[Cost]-[Actual Cost]";

project.ExtendedAttributes.Add(definition);

var task = project.RootTask.Children.Add("Task");
task.Set(Tsk.Start, new DateTime(2020, 4, 21, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(1, TimeUnitType.Day));
task.Set(Tsk.Finish, new DateTime(2020, 4, 21, 17, 0, 0));
task.Set(Tsk.Deadline, new DateTime(2020, 4, 22, 17, 0, 0));
task.Set(Tsk.Cost, 20);
task.Set(Tsk.ActualCost, 13);

// Crear atributo extendido
var extendedAttribute = definition.CreateExtendedAttribute();
task.ExtendedAttributes.Add(extendedAttribute);

Console.WriteLine("Before change:");
Console.WriteLine("Alias: " + definition.Alias);
Console.WriteLine("Field Id: " + extendedAttribute.FieldId);
Console.WriteLine("Value: " + extendedAttribute.NumericValue);

// crear una nueva definición de atributo extendido de fecha
var newDefinition = ExtendedAttributeDefinition.CreateTaskDefinition(CustomFieldType.Date, ExtendedAttributeTask.Date1, string.Empty);

// Agregar una fórmula al atributo.
newDefinition.Alias = "Days from finish to deadline";
newDefinition.Formula = "[Deadline] - [Finish]";
project.ExtendedAttributes.Add(newDefinition);

extendedAttribute = newDefinition.CreateExtendedAttribute();

Console.WriteLine();
Console.WriteLine("After change:");
Console.WriteLine("Alias: " + definition.Alias);
Console.WriteLine("Field Id: " + extendedAttribute.FieldId);
Console.WriteLine("Value: " + extendedAttribute.DateValue.Day);
```

### Ver también

* class [ExtendedAttribute](../)
* namespace [Aspose.Tasks](../../extendedattribute/)
* assembly [Aspose.Tasks](../../../)


