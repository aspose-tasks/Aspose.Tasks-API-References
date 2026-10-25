---
title: "Enumeración GraphicalIndicatorCriteriaType"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Enumeración Aspose.Tasks.GraphicalIndicatorCriteriaType. Representa la ubicación de los criterios del indicador gráfico"
type: docs
weight: 740
url: /es/net/aspose.tasks/graphicalindicatorcriteriatype/
---
## GraphicalIndicatorCriteriaType enumeration

Representa la ubicación de los criterios del indicador gráfico.

```csharp
public enum GraphicalIndicatorCriteriaType
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| NonSummaryRows | `0` | Representa filas no resumidas. |
| SummaryRows | `1` | Representa filas resumidas. |
| ProjectSummary | `2` | Representa la fila de tarea resumida del proyecto. |

## Ejemplos

Muestra cómo configurar un indicador gráfico para un atributo extendido.

```csharp
Project project = new Project();

var def = ExtendedAttributeDefinition.CreateTaskDefinition(ExtendedAttributeTask.Number1, "Number field");
project.ExtendedAttributes.Add(def);
def.GraphicalIndicator = new GraphicalIndicatorsInfo();

GraphicalIndicatorCriteria criteria1 = new GraphicalIndicatorCriteria(
    GraphicalIndicatorCriteriaType.SummaryRows,
    FilterComparisonType.IsLessThan,
    2,
    new GraphicalIndicatorCriteriaValue(100m));

// El criterio 'IsWithin' requiere 2 valores.
GraphicalIndicatorCriteria criteria2 = new GraphicalIndicatorCriteria(
    GraphicalIndicatorCriteriaType.SummaryRows,
    FilterComparisonType.IsWithin,
    4,
    new GraphicalIndicatorCriteriaValue(101),
    new GraphicalIndicatorCriteriaValue(1000m));

// El criterio 'IsAnyValue' no requiere valores.
GraphicalIndicatorCriteria criteria3 = new GraphicalIndicatorCriteria(
    GraphicalIndicatorCriteriaType.SummaryRows,
    FilterComparisonType.IsAnyValue,
    4,
    null);

def.GraphicalIndicator.Criteria.Add(criteria1);
def.GraphicalIndicator.Criteria.Add(criteria2);
def.GraphicalIndicator.Criteria.Add(criteria3);

def.GraphicalIndicator.ProjectSummaryInheritFromNonSummaryRows = true;
def.GraphicalIndicator.SummaryRowsInheritFromNonSummaryRows = true;
def.GraphicalIndicator.ShowDataValuesInTooltip = false;

project.Save(OutDir + "CreateGraphicalIndicators_out.mpp", SaveFileFormat.Mpp);
```

### Ver también

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


