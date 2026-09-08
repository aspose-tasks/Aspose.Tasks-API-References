---
title: "Project.GlobalizationSettings"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Propiedad de Project. Obtiene o establece la configuración de globalización específica del idioma del proyecto"
type: docs
weight: 460
url: /es/net/aspose.tasks/project/globalizationsettings/
---
## Project.GlobalizationSettings property

Obtiene o establece la configuración de globalización (específica de idioma) del proyecto.

```csharp
public GlobalizationSettings GlobalizationSettings { get; set; }
```

## Observaciones

La forma recomendada es usar literales o formatos independientes de la cultura en todo el proyecto. Sin embargo, si un proyecto usa literales específicos de la cultura, esta clase puede usarse para ayudar al motor de cálculo a analizar esos literales.

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

* class [GlobalizationSettings](../../globalizationsettings/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


