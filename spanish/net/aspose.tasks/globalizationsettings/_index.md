---
title: "Clase GlobalizationSettings"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Clase Aspose.Tasks.GlobalizationSettings. Representa la configuración de globalización de los proyectos."
type: docs
weight: 720
url: /es/net/aspose.tasks/globalizationsettings/
---
## GlobalizationSettings class

Representa la configuración de globalización del proyecto.

```csharp
public class GlobalizationSettings
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [GlobalizationSettings](globalizationsettings/)() | El constructor predeterminado. |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| virtual [FalseLiteral](../../aspose.tasks/globalizationsettings/falseliteral/) { get; } | Obtiene una cadena para el literal booleano 'false' usado en una fórmula. |
| virtual [FormulaDateNA](../../aspose.tasks/globalizationsettings/formuladatena/) { get; } | Obtiene el literal "NA" (valor vacío) usado en una fórmula para un campo de fecha. |
| virtual [TrueLiteral](../../aspose.tasks/globalizationsettings/trueliteral/) { get; } | Obtiene una cadena para el literal booleano 'true' usado en una fórmula. |

## Observaciones

La forma recomendada es usar literales o formatos independientes de la cultura en todo el proyecto. Sin embargo, si un proyecto usa literales específicos de la cultura, esta clase puede usarse para ayudar al motor de cálculo de fórmulas a analizar esos literales.

## Ejemplos

Muestra cómo establecer la configuración específica de idioma del proyecto.

```csharp
var project = new Project();

var attribute = ExtendedAttributeDefinition.CreateTaskDefinition(ExtendedAttributeTask.Number1, "Number");
attribute.Formula = "IIf(ProjDateValue('n.a.')=[Date1];100;200)";

project.ExtendedAttributes.Add(attribute);

var task = project.RootTask.Children.Add("Task");

// Crear atributo extendido
var extendedAttribute = attribute.CreateExtendedAttribute();
task.ExtendedAttributes.Add(extendedAttribute);

var attributeDate = ExtendedAttributeDefinition.CreateTaskDefinition(ExtendedAttributeTask.Date1, "Date");

task.ExtendedAttributes.Add(attributeDate.CreateExtendedAttribute(DateTime.MinValue));

Console.WriteLine(extendedAttribute.NumericValue);

project.GlobalizationSettings = new MyGlobalizationSettings();

Console.WriteLine(extendedAttribute.NumericValue);
```

### Ver también

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


