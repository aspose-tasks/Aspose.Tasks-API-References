---
title: "Filter.Criteria"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Filter 속성. 작업 또는 리소스가 MSP 보기에서 표시되기 위해 충족해야 하는 기준을 가져오거나 설정합니다."
type: docs
weight: 20
url: /ko/net/aspose.tasks/filter/criteria/
---
## Filter.Criteria property

MSP 보기에서 표시되기 위해 작업 또는 리소스가 충족해야 하는 기준을 가져오거나 설정합니다.

```csharp
public FilterCriteria Criteria { get; set; }
```

## 예제

작업 필터를 읽는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "Project2003.mpp");

var filter = project.TaskFilters.ToList()[1];
Console.WriteLine(filter.Criteria.CriteriaRows.Count);
Console.WriteLine(filter.Criteria.Operation.ToString());

var criteria1 = filter.Criteria.CriteriaRows[0];
Console.WriteLine(criteria1.Test.ToString());
Console.WriteLine(criteria1.Field.ToString());
Console.WriteLine(criteria1.Values[0].ToString());

var criteria2 = filter.Criteria.CriteriaRows[1];
Console.WriteLine(criteria2.Operation.ToString());
Console.WriteLine(criteria2.CriteriaRows.Count);

var criteria21 = criteria2.CriteriaRows[0];
Console.WriteLine(criteria21.Test.ToString());
Console.WriteLine(criteria21.Field.ToString());
Console.WriteLine(criteria21.Values[0].ToString());

var criteria22 = criteria2.CriteriaRows[1];
Console.WriteLine(criteria22.Test.ToString());
Console.WriteLine(criteria22.Field.ToString());
Console.WriteLine(criteria22.Values[0].ToString());
Console.WriteLine(filter.Criteria);
```

### 또 보기

* class [FilterCriteria](../../filtercriteria/)
* class [Filter](../)
* namespace [Aspose.Tasks](../../filter/)
* assembly [Aspose.Tasks](../../../)


