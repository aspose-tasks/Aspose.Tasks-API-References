---
title: "Clase ExtendedAttribute"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Aspose.Tasks.ExtendedAttribute clase. Representa atributos extendidos"
type: docs
weight: 520
url: /es/net/aspose.tasks/extendedattribute/
---
## ExtendedAttribute class

Representa atributos extendidos.

```csharp
public class ExtendedAttribute
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [AttributeDefinition](../../aspose.tasks/extendedattribute/attributedefinition/) { get; } | Obtiene la definición del atributo. |
| [DateValue](../../aspose.tasks/extendedattribute/datevalue/) { get; set; } | Obtiene o establece un valor para atributos con tipos de fecha (Date, Start, Finish). |
| [DurationValue](../../aspose.tasks/extendedattribute/durationvalue/) { get; set; } | Obtiene o establece el valor para atributos con tipo 'Duration'. |
| [FieldId](../../aspose.tasks/extendedattribute/fieldid/) { get; } | Obtiene el id de un campo. |
| [FlagValue](../../aspose.tasks/extendedattribute/flagvalue/) { get; set; } | Obtiene o establece un valor que indica si una bandera está establecida para un atributo con tipo 'Flag'. |
| [IsErrorValue](../../aspose.tasks/extendedattribute/iserrorvalue/) { get; } | Obtiene si el cálculo del valor del atributo extendido resultó en un error. |
| [NumericValue](../../aspose.tasks/extendedattribute/numericvalue/) { get; set; } | Obtiene o establece un valor para atributos con tipos numéricos (Cost, Number). |
| [TextValue](../../aspose.tasks/extendedattribute/textvalue/) { get; set; } | Obtiene o establece un valor para atributos con tipo 'Text'. |
| [ValueGuid](../../aspose.tasks/extendedattribute/valueguid/) { get; } | Obtiene el guid de un valor de búsqueda. |
| [ValueReadOnly](../../aspose.tasks/extendedattribute/valuereadonly/) { get; } | Obtiene un valor que indica si el valor de esta instancia `ExtendedAttribute` es de solo lectura. devuelve true si una fórmula o acumulación está definida en el [`ExtendedAttributeDefinition`](../extendedattributedefinition/) para este objeto. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| override [ToString](../../aspose.tasks/extendedattribute/tostring/)() | Devuelve la representación corta en cadena de un atributo extendido. |

## Observaciones

Actualmente se admiten todos los tipos de atributos Extended al leer desde MSP Xml 2003/2007 y mpp 2003. Para MSP mpp 2007 se admiten todas las lecturas de atributos Extended excepto duraciones y banderas.

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


