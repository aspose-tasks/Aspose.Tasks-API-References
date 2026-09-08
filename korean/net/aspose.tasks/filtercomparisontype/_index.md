---
title: "열거형 FilterComparisonType"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Aspose.Tasks.FilterComparisonType 열거형. FieldName과 Value 사이에 수행되는 비교 유형으로, 필터 또는 그래픽 표시기의 선택 기준으로 작동합니다."
type: docs
weight: 620
url: /ko/net/aspose.tasks/filtercomparisontype/
---
## FilterComparisonType enumeration

필터 또는 그래픽 표시기의 선택 기준으로 작동하는 FieldName과 Value 사이에 수행되는 비교 유형을 지정합니다.

```csharp
public enum FilterComparisonType
```

### 값들

| 이름 | 값 | 설명 |
| --- | --- | --- |
| Equals | `6` | Field의 값이 Value와 같습니다. |
| DoesNotEqual | `7` | Field의 값이 Value와 같지 않습니다. |
| IsGreaterThan | `2` | Field의 값이 Value보다 큽니다. |
| IsGreaterThanOrEqualTo | `4` | Field의 값이 Value보다 크거나 같습니다. |
| IsLessThan | `3` | Field의 값이 Value보다 작습니다. |
| IsLessThanOrEqualTo | `5` | Field의 값이 Value보다 작거나 같습니다. |
| IsWithin | `1` | Field의 값이 Value 범위 내에 있습니다. |
| IsNotWithin | `9` | Field의 값이 Value 범위 내에 없습니다. |
| Contains | `8` | Field의 값에 Value가 포함됩니다. |
| DoesNotContain | `10` | Field의 값에 Value가 포함되지 않습니다. |
| ContainsExactly | `11` | Field의 값에 Value가 정확히 포함됩니다. |
| IsOneOf | `12` | Field의 값이 지정된 Values 중 하나와 같습니다. AutoFilters에서 사용됩니다. |
| Undefined | `0` | 정의되지 않은 값입니다. |
| IsAnyValue | `255` | 'Is any value' 조건. 그래픽 표시기에 적용됩니다. |

## 예제

작업 필터 기준을 읽는 방법을 보여줍니다.

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

// 필터 기준을 문자열로 출력합니다.
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

### 또 보기

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


