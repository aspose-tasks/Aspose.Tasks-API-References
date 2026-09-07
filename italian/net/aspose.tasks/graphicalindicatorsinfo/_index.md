---
title: "Classe GraphicalIndicatorsInfo"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Classe Aspose.Tasks.GraphicalIndicatorsInfo. Rappresenta una definizione di indicatori grafici associata a un attributo esteso."
type: docs
weight: 760
url: /it/net/aspose.tasks/graphicalindicatorsinfo/
---
## GraphicalIndicatorsInfo class

Rappresenta una definizione di indicatori grafici associata a un attributo esteso.

```csharp
public sealed class GraphicalIndicatorsInfo
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [GraphicalIndicatorsInfo](graphicalindicatorsinfo/)() | Inizializza una nuova istanza del tipo `GraphicalIndicatorsInfo`. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [Criteria](../../aspose.tasks/graphicalindicatorsinfo/criteria/) { get; } | Ottiene un elenco di criteri dell'indicatore grafico. |
| [ProjectSummaryInheritFromNonSummaryRows](../../aspose.tasks/graphicalindicatorsinfo/projectsummaryinheritfromnonsummaryrows/) { get; set; } | Ottiene o imposta il flag che indica se la riga di riepilogo del progetto eredita i criteri dalle righe di riepilogo. |
| [ShowDataValuesInTooltip](../../aspose.tasks/graphicalindicatorsinfo/showdatavaluesintooltip/) { get; set; } | Ottiene o imposta il flag che indica se i valori dei dati per il campo devono essere mostrati nei tooltip. |
| [SummaryRowsInheritFromNonSummaryRows](../../aspose.tasks/graphicalindicatorsinfo/summaryrowsinheritfromnonsummaryrows/) { get; set; } | Ottiene o imposta il flag che indica se le righe di riepilogo ereditano i criteri dalle righe non di riepilogo. |

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


