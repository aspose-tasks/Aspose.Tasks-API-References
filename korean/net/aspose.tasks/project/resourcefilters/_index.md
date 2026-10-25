---
title: "Project.ResourceFilters"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Project 속성. 모든 리소스 기반 필터 정의를 가져옵니다. ResourceFilters는 Filter 객체의 컬렉션입니다."
type: docs
weight: 760
url: /ko/net/aspose.tasks/project/resourcefilters/
---
## Project.ResourceFilters property

모든 리소스 기반 필터 정의를 가져옵니다. ResourceFilters는 [`Filter`](../../filter/) 객체의 컬렉션입니다.

```csharp
public FilterCollection ResourceFilters { get; }
```

## 예제

작업/리소스 필터 정의를 읽는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "ReadFilterDefinitionData.mpp");
List<Filter> taskFilters = project.TaskFilters.ToList();
Console.WriteLine("Task Filters Count: " + taskFilters.Count);
Console.WriteLine("All Tasks: " + taskFilters[0].Name);
Console.WriteLine("Task Item: " + taskFilters[0].FilterType);
Console.WriteLine("Task Filters Show In Menu: " + taskFilters[0].ShowInMenu);
Console.WriteLine("Task filter ShowRelatedSummaryRows: " + taskFilters[0].ShowRelatedSummaryRows);

// 리소스 필터에 접근하기
List<Filter> rscFilters = project.ResourceFilters.ToList();
Console.WriteLine("Project.ResourceFilters count: " + rscFilters.Count);
Console.WriteLine("Resource Filter Item Type: Item.ResourceType: " + rscFilters[0].FilterType);
Console.WriteLine("Resource filter ShowInMenu" + rscFilters[0].ShowInMenu);
Console.WriteLine("Resource filter ShowRelatedSummaryRows: " + rscFilters[0].ShowRelatedSummaryRows);
```

### 또 보기

* class [FilterCollection](../../filtercollection/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


