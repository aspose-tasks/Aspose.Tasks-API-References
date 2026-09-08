---
title: "Класс GraphicalIndicatorsInfo"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Класс Aspose.Tasks.GraphicalIndicatorsInfo. Представляет определение графических индикаторов, связанное с расширенным атрибутом"
type: docs
weight: 760
url: /ru/net/aspose.tasks/graphicalindicatorsinfo/
---
## GraphicalIndicatorsInfo class

Представляет определение графических индикаторов, связанное с расширенным атрибутом.

```csharp
public sealed class GraphicalIndicatorsInfo
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [GraphicalIndicatorsInfo](graphicalindicatorsinfo/)() | Инициализирует новый экземпляр типа `GraphicalIndicatorsInfo`. |

## Свойства

| Имя | Описание |
| --- | --- |
| [Criteria](../../aspose.tasks/graphicalindicatorsinfo/criteria/) { get; } | Возвращает список критериев графических индикаторов. |
| [ProjectSummaryInheritFromNonSummaryRows](../../aspose.tasks/graphicalindicatorsinfo/projectsummaryinheritfromnonsummaryrows/) { get; set; } | Получает или задает флаг, указывающий, наследует ли строка сводки проекта критерии от строк сводки. |
| [ShowDataValuesInTooltip](../../aspose.tasks/graphicalindicatorsinfo/showdatavaluesintooltip/) { get; set; } | Получает или задает флаг, указывающий, должны ли значения данных поля отображаться во всплывающих подсказках. |
| [SummaryRowsInheritFromNonSummaryRows](../../aspose.tasks/graphicalindicatorsinfo/summaryrowsinheritfromnonsummaryrows/) { get; set; } | Получает или задает флаг, указывающий, наследуют ли строки сводки критерии от несводных строк. |

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


