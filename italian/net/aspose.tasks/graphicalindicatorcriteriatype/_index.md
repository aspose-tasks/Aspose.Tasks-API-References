---
title: "Enumerazione GraphicalIndicatorCriteriaType"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Enumerazione Aspose.Tasks.GraphicalIndicatorCriteriaType. Rappresenta il posizionamento dei criteri dell'indicatore grafico"
type: docs
weight: 740
url: /it/net/aspose.tasks/graphicalindicatorcriteriatype/
---
## GraphicalIndicatorCriteriaType enumeration

Rappresenta la posizione dei criteri dell'indicatore grafico.

```csharp
public enum GraphicalIndicatorCriteriaType
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| NonSummaryRows | `0` | Rappresenta righe non di riepilogo. |
| SummaryRows | `1` | Rappresenta righe di riepilogo. |
| ProjectSummary | `2` | Rappresenta la riga del compito di riepilogo del progetto. |

## Esempi

Mostra come configurare un indicatore grafico per un attributo esteso.

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

// Il criterio 'IsWithin' richiede 2 valori.
GraphicalIndicatorCriteria criteria2 = new GraphicalIndicatorCriteria(
    GraphicalIndicatorCriteriaType.SummaryRows,
    FilterComparisonType.IsWithin,
    4,
    new GraphicalIndicatorCriteriaValue(101),
    new GraphicalIndicatorCriteriaValue(1000m));

// Il criterio 'IsAnyValue' non richiede valori.
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

### Vedi anche

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


