---
title: "Class FilterCriteria"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Aspose.Tasks.FilterCriteria 클래스. 작업 또는 리소스가 MSP 보기에서 표시되기 위해 충족해야 하는 기준을 정의합니다."
type: docs
weight: 630
url: /ko/net/aspose.tasks/filtercriteria/
---
## FilterCriteria class

MSP 보기에서 표시되기 위해 작업 또는 리소스가 충족해야 하는 기준을 정의합니다.

```csharp
public class FilterCriteria
```

## 생성자

| 이름 | 설명 |
| --- | --- |
| [FilterCriteria](filtercriteria/)() | 기본 생성자입니다. |

## 속성

| 이름 | 설명 |
| --- | --- |
| [CriteriaRows](../../aspose.tasks/filtercriteria/criteriarows/) { get; } | `FilterCriteria` 자식 행 목록을 가져옵니다. 필터에 기준 행이 두 개 이상 포함된 경우 And 연산자의 효과는 두 행의 기준을 모두 충족해야 작업 또는 리소스가 이 필터의 결과로 표시된다는 것입니다. Or 연산자의 효과는 두 행 중 하나의 기준만 충족하면 된다는 것입니다. |
| [Field](../../aspose.tasks/filtercriteria/field/) { get; set; } | 변경할 [`Field`](./field/)를 가져오거나 설정합니다. |
| [Operation](../../aspose.tasks/filtercriteria/operation/) { get; set; } | FieldName, Test 및 Value로 설정된 기준을 가져오거나 설정하며, 이는 필터의 다른 기준과 관련됩니다. |
| [Test](../../aspose.tasks/filtercriteria/test/) { get; set; } | 필터의 선택 기준으로 작용하는 FieldName과 Value 사이의 비교 유형을 가져오거나 설정합니다. [`FilterComparisonType`](../filtercomparisontype/) |
| [Values](../../aspose.tasks/filtercriteria/values/) { get; } | FieldName으로 지정된 필드 값과 비교할 객체 값을 가져옵니다. |

## 메서드

| 이름 | 설명 |
| --- | --- |
| [IsFieldValue](../../aspose.tasks/filtercriteria/isfieldvalue/)() | FilterCriteria의 오른쪽 값이 상수 값이 아닌 필드 참조인지 여부를 가져옵니다. |
| [SetValueField](../../aspose.tasks/filtercriteria/setvaluefield/)(Field) | FieldName으로 지정된 필드 값과 비교될 필드를 설정합니다. |
| override [ToString](../../aspose.tasks/filtercriteria/tostring/)() | `FilterCriteria` 클래스 인스턴스의 문자열 표현을 반환합니다. |

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


