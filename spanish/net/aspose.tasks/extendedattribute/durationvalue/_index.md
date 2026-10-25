---
title: "ExtendedAttribute.DurationValue"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Propiedad ExtendedAttribute. Obtiene o establece el valor para atributos con tipo Duración"
type: docs
weight: 30
url: /es/net/aspose.tasks/extendedattribute/durationvalue/
---
## ExtendedAttribute.DurationValue property

Obtiene o establece el valor para atributos con tipo 'Duration'.

```csharp
public Duration DurationValue { get; set; }
```

### Excepciones

| excepción | condición |
| --- | --- |
| InvalidOperationException | Se lanza si la propiedad [`AttributeDefinition`](../attributedefinition/) no está inicializada o el tipo de campo personalizado de la propiedad [`AttributeDefinition`](../attributedefinition/) no es una instancia de [`Duration`](../../duration/). |

## Ejemplos

Muestra cómo agregar atributos extendidos que utilizan fórmulas de fecha/hora de MS Project.

```csharp
var project = new Project();
var task = project.RootTask.Children.Add("Task");

var numberDefinition = ExtendedAttributeDefinition.CreateTaskDefinition(ExtendedAttributeTask.Number1, null);
project.ExtendedAttributes.Add(numberDefinition);

var numberAttribute = numberDefinition.CreateExtendedAttribute();
task.ExtendedAttributes.Add(numberAttribute);

// Establecer la fórmula ProjDateDiff e imprimir el valor del atributo extendido
numberDefinition.Formula = "ProjDateDiff(\"03/23/2015\",\"03/18/2015\")";
Console.WriteLine(numberAttribute.NumericValue);
numberDefinition.Formula = "ProjDateDiff(\"03/23/2015\",\"03/25/2015\")";
Console.WriteLine(numberAttribute.NumericValue);

var dateDefinition = ExtendedAttributeDefinition.CreateTaskDefinition(ExtendedAttributeTask.Date1, null);
project.ExtendedAttributes.Add(dateDefinition);
var dateAttribute = dateDefinition.CreateExtendedAttribute();
task.ExtendedAttributes.Add(dateAttribute);

var durationDefinition = ExtendedAttributeDefinition.CreateTaskDefinition(ExtendedAttributeTask.Duration4, "Custom duration field");
project.ExtendedAttributes.Add(durationDefinition);
var durationAttribute = durationDefinition.CreateExtendedAttribute();
task.ExtendedAttributes.Add(durationAttribute);

var textDefinition = ExtendedAttributeDefinition.CreateTaskDefinition(ExtendedAttributeTask.Text5, "Custom text field");
project.ExtendedAttributes.Add(textDefinition);
var textAttribute = textDefinition.CreateExtendedAttribute();
task.ExtendedAttributes.Add(textAttribute);

// Establecer la fórmula ProjDateSub e imprimir el valor del atributo extendido
dateDefinition.Formula = "ProjDateSub(\"3/19/2015\", \"1d\")";
Console.WriteLine(dateAttribute.DateValue);

// Podemos establecer la fórmula ProjDurConv en un atributo con valor de duración así como en un atributo con valor de texto.
// Establecer la fórmula ProjDurConv en un atributo extendido con valor de duración e imprimir su valor.
durationDefinition.Formula = "ProjDurConv([Duration], pjHours)";
Console.WriteLine(durationAttribute.DurationValue);

// Establecer la fórmula ProjDurConv en un atributo extendido con valor de texto e imprimir su valor.
textDefinition.Formula = "ProjDurConv([Duration], pjWeeks)";
Console.WriteLine(textAttribute.TextValue);

// Establecer la fórmula Second e imprimir el valor del atributo extendido
numberDefinition.Formula = "Second(\"4/21/2015 2:53:41 AM\")";
Console.WriteLine(numberAttribute.NumericValue);

// Establecer la fórmula Weekday e imprimir el valor del atributo extendido
numberDefinition.Formula = "Weekday(\"24/3/2015\", 1)";
Console.WriteLine(numberAttribute.NumericValue);
numberDefinition.Formula = "Weekday(\"24/3/2015\", 2)";
Console.WriteLine(numberAttribute.NumericValue);
numberDefinition.Formula = "Weekday(\"24/3/2015\", 3)";
Console.WriteLine(numberAttribute.NumericValue);
```

### Ver también

* struct [Duration](../../duration/)
* class [ExtendedAttribute](../)
* namespace [Aspose.Tasks](../../extendedattribute/)
* assembly [Aspose.Tasks](../../../)


