---
title: "Project.TaskFilters"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Project 속성. 모든 작업 기반 필터 정의를 가져옵니다. TaskFilters는 Filter 객체의 컬렉션입니다."
type: docs
weight: 910
url: /ko/net/aspose.tasks/project/taskfilters/
---
## Project.TaskFilters property

모든 작업 기반 필터 정의를 가져옵니다. TaskFilters는 [`Filter`](../../filter/) 객체의 컬렉션입니다.

```csharp
public FilterCollection TaskFilters { get; }
```

## 예제

프로젝트 작업 필터를 읽는 방법을 보여줍니다.

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

* class [FilterCollection](../../filtercollection/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


