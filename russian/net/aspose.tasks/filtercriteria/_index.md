---
title: "Класс FilterCriteria"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Класс Aspose.Tasks.FilterCriteria. Определяет критерии, которым задачи или ресурсы должны соответствовать, чтобы отображаться в представлении MSP"
type: docs
weight: 630
url: /ru/net/aspose.tasks/filtercriteria/
---
## FilterCriteria class

Определяет критерии, которым задачи или ресурсы должны соответствовать, чтобы отображаться в представлении MSP.

```csharp
public class FilterCriteria
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [FilterCriteria](filtercriteria/)() | Конструктор по умолчанию. |

## Свойства

| Имя | Описание |
| --- | --- |
| [CriteriaRows](../../aspose.tasks/filtercriteria/criteriarows/) { get; } | Получает список дочерних строк `FilterCriteria`. Если фильтр содержит более одной строки критериев, то действие оператора И заключается в том, что критерии обеих строк должны быть выполнены, чтобы задача или ресурс отобразились в результате этого фильтра. Действие оператора ИЛИ заключается в том, что критерий одной из строк должен быть выполнен. |
| [Field](../../aspose.tasks/filtercriteria/field/) { get; set; } | Получает или задает [`Field`](./field/) для изменения. |
| [Operation](../../aspose.tasks/filtercriteria/operation/) { get; set; } | Получает или задает критерий, установленный с помощью FieldName, Test и Value, относящийся к другим критериям в фильтре. |
| [Test](../../aspose.tasks/filtercriteria/test/) { get; set; } | Получает или задает тип сравнения между FieldName и Value, который служит в качестве критериев выбора для фильтра. [`FilterComparisonType`](../filtercomparisontype/) |
| [Values](../../aspose.tasks/filtercriteria/values/) { get; } | Получает объектные значения для сравнения со значением поля, указанного в FieldName. |

## Методы

| Имя | Описание |
| --- | --- |
| [IsFieldValue](../../aspose.tasks/filtercriteria/isfieldvalue/)() | Определяет, является ли правое значение FilterCriteria ссылкой на поле, а не константным значением. |
| [SetValueField](../../aspose.tasks/filtercriteria/setvaluefield/)(Field) | Задает поле, значение которого будет сравниваться со значением поля, указанного в FieldName. |
| override [ToString](../../aspose.tasks/filtercriteria/tostring/)() | Возвращает строковое представление экземпляра класса `FilterCriteria`. |

## Примеры

Показывает, как читать критерии фильтра задач.

```csharp
var project = new Project(DataDir + "Project2003.mpp");

var filter = project.TaskFilters.ToList()[1];
Console.WriteLine("Count of criteria rows: " + filter.Criteria.CriteriaRows.Count);
foreach (var row in filter.Criteria.CriteriaRows)
{
    Console.WriteLine("Field: " + row.Field);
    Console.WriteLine("Operation: " + row.Operation);
    Console.WriteLine("Test: " + row.Test);

    var values = row.Values.Where(c => c != null).ToArray();
    if (values.Length == 0)
    {
        continue;
    }

    Console.WriteLine("Value{0}: {1}", values.Length == 1 ? "" : "s", string.Join(", ", values));
}

// Печать критериев фильтра в виде строки
Console.WriteLine(filter.Criteria.Operation.ToString());

var criteria1 = filter.Criteria.CriteriaRows[0];
Console.WriteLine("Criteria filter 1:");
Console.WriteLine(criteria1.ToString());

var criteria2 = filter.Criteria.CriteriaRows[1];
Console.WriteLine(criteria2.Operation.ToString());
Console.WriteLine(criteria2.CriteriaRows.Count);
Console.WriteLine("Criteria filter 2:");
Console.WriteLine(criteria2.ToString());

var criteria21 = criteria2.CriteriaRows[0];
Console.WriteLine("Criteria filter 21:");
Console.WriteLine(criteria21.ToString());

var criteria22 = criteria2.CriteriaRows[1];
Console.WriteLine("Criteria filter 22:");
Console.WriteLine(criteria22.ToString());
```

### См. также

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


