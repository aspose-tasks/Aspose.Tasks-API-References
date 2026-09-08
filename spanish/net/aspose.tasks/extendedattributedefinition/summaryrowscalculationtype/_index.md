---
title: "ExtendedAttributeDefinition.SummaryRowsCalculationType"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Propiedad ExtendedAttributeDefinition. Obtiene o establece el tipo de cálculo del valor de los atributos personalizados para filas de resumen"
type: docs
weight: 260
url: /es/net/aspose.tasks/extendedattributedefinition/summaryrowscalculationtype/
---
## ExtendedAttributeDefinition.SummaryRowsCalculationType property

Obtiene o establece el tipo de cálculo del valor del atributo personalizado para filas de resumen.

```csharp
public SummaryRowsCalculationType SummaryRowsCalculationType { get; set; }
```

## Ejemplos

Muestra cómo trabajar con el tipo de cálculo de una definición de atributo extendido.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");
task.Set(Tsk.Start, new DateTime(2020, 4, 16, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(1, TimeUnitType.Day));

// crear definición de atributo con tipo 'Formula' donde los valores para tareas hoja y tareas resumen se calculan usando una fórmula.
var calculation = ExtendedAttributeDefinition.CreateTaskDefinition(ExtendedAttributeTask.Date5, null);
calculation.CalculationType = CalculationType.Formula;
calculation.SummaryRowsCalculationType = SummaryRowsCalculationType.UseFormula;
calculation.Formula = "[stARt]";
project.ExtendedAttributes.Add(calculation);

// crear definición de atributo donde los valores para tareas resumen se calculan usando el tipo de acumulación 'Average'.
var lookup = ExtendedAttributeDefinition.CreateTaskDefinition(ExtendedAttributeTask.Cost1, null);
lookup.SummaryRowsCalculationType = SummaryRowsCalculationType.Rollup;
lookup.RollupType = RollupType.Average;
project.ExtendedAttributes.Add(lookup);
```

### Ver también

* enum [SummaryRowsCalculationType](../../summaryrowscalculationtype/)
* class [ExtendedAttributeDefinition](../)
* namespace [Aspose.Tasks](../../extendedattributedefinition/)
* assembly [Aspose.Tasks](../../../)


