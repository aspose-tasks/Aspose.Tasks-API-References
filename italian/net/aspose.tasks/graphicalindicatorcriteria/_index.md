---
title: "Classe GraphicalIndicatorCriteria"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Classe Aspose.Tasks.GraphicalIndicatorCriteria. Rappresenta un criterio di indicatore grafico associato a un attributo esteso"
type: docs
weight: 730
url: /it/net/aspose.tasks/graphicalindicatorcriteria/
---
## GraphicalIndicatorCriteria class

Rappresenta un criterio di indicatore grafico associato a un attributo esteso.

```csharp
public sealed class GraphicalIndicatorCriteria
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [GraphicalIndicatorCriteria](graphicalindicatorcriteria/#constructor)(GraphicalIndicatorCriteriaType, FilterComparisonType, int, GraphicalIndicatorCriteriaValue) | Inizializza una nuova istanza del tipo `GraphicalIndicatorCriteria`. |
| [GraphicalIndicatorCriteria](graphicalindicatorcriteria/#constructor_1)(GraphicalIndicatorCriteriaType, FilterComparisonType, int, GraphicalIndicatorCriteriaValue, GraphicalIndicatorCriteriaValue) | Inizializza una nuova istanza del tipo `GraphicalIndicatorCriteria`. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [ImageIndex](../../aspose.tasks/graphicalindicatorcriteria/imageindex/) { get; } | Ottiene l'indice dell'immagine da visualizzare quando il campo soddisfa i criteri. |
| [RowType](../../aspose.tasks/graphicalindicatorcriteria/rowtype/) { get; } | Ottiene il valore dell'enumerazione [`GraphicalIndicatorCriteriaType`](../graphicalindicatorcriteriatype/) che indica per quali righe viene applicato l'indicatore. |
| [Test](../../aspose.tasks/graphicalindicatorcriteria/test/) { get; } | Ottiene il tipo di confronto effettuato tra il valore dell'attributo esteso e i valori che fungono da criterio per l'applicazione dell'indicatore grafico. [`FilterComparisonType`](../filtercomparisontype/) |
| [Value1](../../aspose.tasks/graphicalindicatorcriteria/value1/) { get; } | Ottiene il valore usato per testare il valore dell'attributo esteso. |
| [Value2](../../aspose.tasks/graphicalindicatorcriteria/value2/) { get; } | Ottiene il secondo valore usato per testare il valore dell'attributo esteso nel caso dei tipi di confronto 'IsWithin' e 'IsNotWithin'. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| override [ToString](../../aspose.tasks/graphicalindicatorcriteria/tostring/)() | Restituisce la rappresentazione stringa dell'istanza della classe `GraphicalIndicatorCriteria`. |

## Esempi

Mostra come recuperare le informazioni degli indicatori grafici.

```csharp
Project project = new Project(DataDir + "graphical_indicators.mpp");

foreach (var ea in project.ExtendedAttributes)
{
    if (ea.GraphicalIndicator == null)
    {
        continue;
    }

    Console.WriteLine("GI for field '{0}':", ea.FieldName);

    foreach (var criterion in ea.GraphicalIndicator.Criteria)
    {
        Console.WriteLine("Row type: {0}", criterion.RowType);
        Console.WriteLine("Image index: {0}", criterion.ImageIndex);
        Console.Write(criterion.Test);
        if (criterion.Value1 != null)
        {
            Console.Write(" ");
            Console.Write(criterion.Value1.RawValue);
        }

        if (criterion.Value2 != null)
        {
            Console.Write(" ");
            Console.WriteLine(criterion.Value2.RawValue);
        }

        Console.WriteLine();
    }
}
```

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


