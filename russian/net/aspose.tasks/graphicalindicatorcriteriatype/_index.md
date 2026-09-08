---
title: "Перечисление GraphicalIndicatorCriteriaType"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Перечисление Aspose.Tasks.GraphicalIndicatorCriteriaType. Представляет расположение критериев графических индикаторов"
type: docs
weight: 740
url: /ru/net/aspose.tasks/graphicalindicatorcriteriatype/
---
## GraphicalIndicatorCriteriaType enumeration

Представляет расположение критериев графического индикатора.

```csharp
public enum GraphicalIndicatorCriteriaType
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| NonSummaryRows | `0` | Представляет строки без итогов. |
| SummaryRows | `1` | Представляет строки с итогами. |
| ProjectSummary | `2` | Представляет строку задачи‑итога проекта. |

## Примеры

Показывает, как настроить графический индикатор для расширенного атрибута.

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

// Критерию 'IsWithin' требуется 2 значения.
GraphicalIndicatorCriteria criteria2 = new GraphicalIndicatorCriteria(
    GraphicalIndicatorCriteriaType.SummaryRows,
    FilterComparisonType.IsWithin,
    4,
    new GraphicalIndicatorCriteriaValue(101),
    new GraphicalIndicatorCriteriaValue(1000m));

// Критерию 'IsAnyValue' не требуются значения.
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

### См. также

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


