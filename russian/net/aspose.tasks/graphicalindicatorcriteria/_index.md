---
title: "Класс GraphicalIndicatorCriteria"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Класс Aspose.Tasks.GraphicalIndicatorCriteria. Представляет один критерий графического индикатора, связанный с расширенным атрибутом"
type: docs
weight: 730
url: /ru/net/aspose.tasks/graphicalindicatorcriteria/
---
## GraphicalIndicatorCriteria class

Представляет один критерий графического индикатора, связанный с расширенным атрибутом.

```csharp
public sealed class GraphicalIndicatorCriteria
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [GraphicalIndicatorCriteria](graphicalindicatorcriteria/#constructor)(GraphicalIndicatorCriteriaType, FilterComparisonType, int, GraphicalIndicatorCriteriaValue) | Инициализирует новый экземпляр типа `GraphicalIndicatorCriteria`. |
| [GraphicalIndicatorCriteria](graphicalindicatorcriteria/#constructor_1)(GraphicalIndicatorCriteriaType, FilterComparisonType, int, GraphicalIndicatorCriteriaValue, GraphicalIndicatorCriteriaValue) | Инициализирует новый экземпляр типа `GraphicalIndicatorCriteria`. |

## Свойства

| Имя | Описание |
| --- | --- |
| [ImageIndex](../../aspose.tasks/graphicalindicatorcriteria/imageindex/) { get; } | Получает индекс изображения для отображения, когда поле соответствует критерию. |
| [RowType](../../aspose.tasks/graphicalindicatorcriteria/rowtype/) { get; } | Получает значение перечисления [`GraphicalIndicatorCriteriaType`](../graphicalindicatorcriteriatype/), которое обозначает, для каких строк применяется индикатор. |
| [Test](../../aspose.tasks/graphicalindicatorcriteria/test/) { get; } | Получает тип сравнения, выполненного между значением расширенного атрибута и значениями, которые служат критерием применения графического индикатора. [`FilterComparisonType`](../filtercomparisontype/) |
| [Value1](../../aspose.tasks/graphicalindicatorcriteria/value1/) { get; } | Получает значение, используемое для проверки значения расширенного атрибута. |
| [Value2](../../aspose.tasks/graphicalindicatorcriteria/value2/) { get; } | Получает второе значение, используемое для проверки значения расширенного атрибута в случае типов сравнения 'IsWithin' и 'IsNotWithin'. |

## Методы

| Имя | Описание |
| --- | --- |
| override [ToString](../../aspose.tasks/graphicalindicatorcriteria/tostring/)() | Возвращает строковое представление экземпляра класса `GraphicalIndicatorCriteria`. |

## Примеры

Показывает, как получить информацию о графических индикаторах.

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


