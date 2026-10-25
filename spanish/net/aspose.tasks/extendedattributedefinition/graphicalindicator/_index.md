---
title: "ExtendedAttributeDefinition.GraphicalIndicator"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Propiedad ExtendedAttributeDefinition. Obtiene o establece información de indicadores gráficos asociada al atributo extendido. Aplicable al formato MPP."
type: docs
weight: 160
url: /es/net/aspose.tasks/extendedattributedefinition/graphicalindicator/
---
## ExtendedAttributeDefinition.GraphicalIndicator property

Obtiene o establece la información de indicadores gráficos asociada al atributo extendido. Aplicable al formato MPP.

```csharp
public GraphicalIndicatorsInfo GraphicalIndicator { get; set; }
```

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

* class [GraphicalIndicatorsInfo](../../graphicalindicatorsinfo/)
* class [ExtendedAttributeDefinition](../)
* namespace [Aspose.Tasks](../../extendedattributedefinition/)
* assembly [Aspose.Tasks](../../../)


