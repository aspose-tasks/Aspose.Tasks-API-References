---
title: "클래스 FilterCollection"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Aspose.Tasks.FilterCollection 클래스. Filter 객체 목록을 포함합니다. ICollectionFilter 인터페이스를 구현합니다."
type: docs
weight: 610
url: /ko/net/aspose.tasks/filtercollection/
---
## FilterCollection class

Contains a list of [`Filter`](../filter/) objects. Implements ICollection&lt;Filter&gt; interface.

```csharp
public class FilterCollection : ICollection<Filter>
```

## 속성

| 이름 | 설명 |
| --- | --- |
| [Count](../../aspose.tasks/filtercollection/count/) { get; } | 이 컬렉션에 포함된 요소 수를 가져옵니다. |
| [IsReadOnly](../../aspose.tasks/filtercollection/isreadonly/) { get; } | 이 컬렉션이 읽기 전용인지 여부를 나타내는 값을 가져옵니다; 그렇지 않으면 false. |

## 메서드

| 이름 | 설명 |
| --- | --- |
| [Add](../../aspose.tasks/filtercollection/add/)(Filter) | 지정된 항목을 이 컬렉션에 추가합니다. |
| [Clear](../../aspose.tasks/filtercollection/clear/)() | 이 컬렉션에서 모든 항목을 제거합니다. |
| [Contains](../../aspose.tasks/filtercollection/contains/)(Filter) | 지정된 항목이 이 컬렉션에 있으면 true를 반환하고, 그렇지 않으면 false를 반환합니다. |
| [CopyTo](../../aspose.tasks/filtercollection/copyto/)(Filter[], int) | 이 컬렉션의 요소를 지정된 배열에 복사하며, 지정된 배열 인덱스부터 시작합니다. |
| [GetEnumerator](../../aspose.tasks/filtercollection/getenumerator/)() | 이 컬렉션에 대한 열거자를 반환합니다. |
| [Remove](../../aspose.tasks/filtercollection/remove/)(Filter) | 이 컬렉션에서 특정 객체의 첫 번째 발생을 제거합니다. |
| [ToList](../../aspose.tasks/filtercollection/tolist/)() | 필터 컬렉션을 [`Filter`](../filter/) 객체 목록으로 변환합니다. |

## 예제

필터 컬렉션을 사용하는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "ReadFilterDefinitionData.mpp");

// 작업 필터를 반복합니다.
Console.WriteLine("Print task filters of {0} project: ", project.Get(Prj.Name));
Console.WriteLine("Task Filters Count: " + project.TaskFilters.Count);
foreach (var filter in project.TaskFilters)
{
    Console.WriteLine("All Tasks: " + filter.Name);
    Console.WriteLine("Task Item: " + filter.FilterType);
    Console.WriteLine("Task Filters Show In Menu: " + filter.ShowInMenu);
    Console.WriteLine("Task filter ShowRelatedSummaryRows: " + filter.ShowRelatedSummaryRows);
    Console.WriteLine();
}

// 리소스 필터를 반복합니다.
Console.WriteLine("Project.ResourceFilters count: " + project.ResourceFilters.Count);
foreach (var filter in project.ResourceFilters)
{
    Console.WriteLine("Resource Filter Item Type: Item.ResourceType: " + filter.FilterType);
    Console.WriteLine("Resource filter ShowInMenu" + filter.ShowInMenu);
    Console.WriteLine("Resource filter ShowRelatedSummaryRows: " + filter.ShowRelatedSummaryRows);
}

var otherProject = new Project(DataDir + "Blank2010.mpp");

// 다른 프로젝트의 필터를 지웁니다.
otherProject.TaskFilters.Clear();

// 필터를 다른 프로젝트에 복사합니다.
var filters = new Filter[project.TaskFilters.Count];
project.TaskFilters.CopyTo(filters, 0);

foreach (var filter in filters)
{
    otherProject.TaskFilters.Add(filter);
}

// 사용자 지정 작업 필터를 추가합니다.
var customFilter = new Filter();
customFilter.Name = "Custom Filter";
customFilter.ShowInMenu = true;
customFilter.ShowRelatedSummaryRows = true;

if (!otherProject.TaskFilters.Contains(customFilter))
{
    if (!otherProject.TaskFilters.IsReadOnly)
    {
        otherProject.TaskFilters.Add(customFilter);
    }
}

// 모든 필터를 제거합니다.
List<Filter> filtersToDelete = otherProject.TaskFilters.ToList();
foreach (var filter in filtersToDelete)
{
    otherProject.TaskFilters.Remove(filter);
}
```

### 또 보기

* class [Filter](../filter/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


