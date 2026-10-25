---
title: "ExtendedAttributeDefinition.GraphicalIndicator"
second_title: "Aspose.Tasks für .NET API-Referenz"
description: "ExtendedAttributeDefinition-Eigenschaft. Ruft Informationen zu grafischen Indikatoren ab oder legt sie fest, die mit dem erweiterten Attribut verknüpft sind. Gültig für das MPP-Format"
type: docs
weight: 160
url: /de/net/aspose.tasks/extendedattributedefinition/graphicalindicator/
---
## ExtendedAttributeDefinition.GraphicalIndicator property

Ruft Informationen zu grafischen Indikatoren ab oder legt sie fest, die mit dem erweiterten Attribut verknüpft sind. Gültig für das MPP-Format.

```csharp
public GraphicalIndicatorsInfo GraphicalIndicator { get; set; }
```

## Beispiele

Zeigt, wie man einen grafischen Indikator für ein erweitertes Attribut einrichtet.

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

// 'IsWithin'-Kriterium erfordert 2 Werte.
GraphicalIndicatorCriteria criteria2 = new GraphicalIndicatorCriteria(
    GraphicalIndicatorCriteriaType.SummaryRows,
    FilterComparisonType.IsWithin,
    4,
    new GraphicalIndicatorCriteriaValue(101),
    new GraphicalIndicatorCriteriaValue(1000m));

// 'IsAnyValue'-Kriterium erfordert keine Werte.
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

### Siehe auch

* class [GraphicalIndicatorsInfo](../../graphicalindicatorsinfo/)
* class [ExtendedAttributeDefinition](../)
* namespace [Aspose.Tasks](../../extendedattributedefinition/)
* assembly [Aspose.Tasks](../../../)


