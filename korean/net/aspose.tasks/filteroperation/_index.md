---
title: "열거형 FilterOperation"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Aspose.Tasks.FilterOperation 열거형. FieldName, FilterComparisonType 및 Value로 설정된 기준이 필터 내 다른 기준과 어떻게 연관되는지를 지정합니다."
type: docs
weight: 640
url: /ko/net/aspose.tasks/filteroperation/
---
## FilterOperation enumeration

FieldName, FilterComparisonType 및 Value로 설정된 기준이 필터 내 다른 기준과 어떻게 관련되는지를 지정합니다.

```csharp
public enum FilterOperation
```

### 값들

| 이름 | 값 | 설명 |
| --- | --- | --- |
| Undefined | `0` | 정의되지 않음. |
| And | `1` | AND 연산자. |
| Or | `2` | OR 연산자. |

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


