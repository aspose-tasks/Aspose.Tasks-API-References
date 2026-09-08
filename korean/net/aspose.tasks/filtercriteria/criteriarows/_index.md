---
title: "FilterCriteria.CriteriaRows"
second_title: "Aspose.Tasks for .NET API 참조"
description: "FilterCriteria 속성. 자식 FilterCriteria 행 목록을 가져옵니다. 필터에 하나 이상의 기준 행이 포함된 경우 And 연산자의 효과는 두 행의 기준이 모두 충족되어야 작업이나 리소스가 이 필터 결과로 표시된다는 것입니다. Or 연산자의 효과는 두 행 중 하나의 기준만 충족되면 된다는 것입니다."
type: docs
weight: 20
url: /ko/net/aspose.tasks/filtercriteria/criteriarows/
---
## FilterCriteria.CriteriaRows property

자식 [`FilterCriteria`](../) 행 목록을 가져옵니다. 필터에 하나 이상의 기준 행이 포함된 경우 And 연산자의 효과는 두 행의 기준이 모두 충족되어야 작업이나 리소스가 이 필터 결과로 표시된다는 것입니다. Or 연산자의 효과는 두 행 중 하나의 기준만 충족되면 된다는 것입니다.

```csharp
public List<FilterCriteria> CriteriaRows { get; }
```

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

* class [FilterCriteria](../)
* namespace [Aspose.Tasks](../../filtercriteria/)
* assembly [Aspose.Tasks](../../../)


