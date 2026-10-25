---
title: "Enumeración RollupType"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Enumeración Aspose.Tasks.RollupType. Especifica el tipo de acumulación"
type: docs
weight: 1950
url: /es/net/aspose.tasks/rolluptype/
---
## RollupType enumeration

Especifica el tipo de consolidación.

```csharp
public enum RollupType
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| Null | `0` | Indica el tipo de acumulación nulo. |
| Maximum | `1` | Indica el tipo de acumulación máximo. |
| Minimum | `2` | Indica el tipo de acumulación mínimo. |
| Count | `3` | Indica el tipo de acumulación de recuento. |
| Sum | `4` | Indica el tipo de acumulación de suma. |
| Average | `5` | Indica el tipo de acumulación de promedio. |
| AverageFirstSublevel | `6` | Indica el tipo de acumulación de promedio del primer subnivel. |
| CountFirstSublevel | `7` | Indica el tipo de acumulación de recuento del primer subnivel. |
| CountNonsummaries | `8` | Indica el tipo de acumulación de recuento de no resúmenes. |

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


