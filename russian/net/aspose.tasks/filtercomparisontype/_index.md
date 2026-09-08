---
title: "Перечисление FilterComparisonType"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Перечисление Aspose.Tasks.FilterComparisonType. Тип сравнения, выполняемый между FieldName и Value, который служит критерием выбора для фильтра или графического индикатора"
type: docs
weight: 620
url: /ru/net/aspose.tasks/filtercomparisontype/
---
## FilterComparisonType enumeration

Тип сравнения между FieldName и Value, который служит критерием выбора для фильтра или графического индикатора.

```csharp
public enum FilterComparisonType
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| Equals | `6` | Значение Field равно Value. |
| DoesNotEqual | `7` | Значение Field не равно Value. |
| IsGreaterThan | `2` | Значение Field больше Value. |
| IsGreaterThanOrEqualTo | `4` | Значение Field больше или равно Value. |
| IsLessThan | `3` | Значение Field меньше Value. |
| IsLessThanOrEqualTo | `5` | Значение Field меньше или равно Value. |
| IsWithin | `1` | Значение Field находится в пределах Value. |
| IsNotWithin | `9` | Значение Field не находится в пределах Value. |
| Contains | `8` | Значение Field содержит Value. |
| DoesNotContain | `10` | Значение Field не содержит Value. |
| ContainsExactly | `11` | Значение Field точно содержит Value. |
| IsOneOf | `12` | Значение Field равно одному из указанных Values. Используется в AutoFilters. |
| Undefined | `0` | Неопределённое значение. |
| IsAnyValue | `255` | Условие 'Is any value'. Применяется к графическим индикаторам. |

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


