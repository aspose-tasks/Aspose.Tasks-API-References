---
title: "FilterCollection.CopyTo"
second_title: "Aspose.Tasks for .NET API 참조"
description: "FilterCollection 메서드. 이 컬렉션의 요소를 지정된 배열 인덱스에서 시작하여 지정된 배열에 복사합니다"
type: docs
weight: 60
url: /ko/net/aspose.tasks/filtercollection/copyto/
---
## FilterCollection.CopyTo method

이 컬렉션의 요소를 지정된 배열에 복사하며, 지정된 배열 인덱스부터 시작합니다.

```csharp
public void CopyTo(Filter[] array, int arrayIndex)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 배열 | Filter[] | 요소를 복사할 지정된 1차원 배열. |
| arrayIndex | Int32 | 복사가 시작되는 지정된 배열의 0 기반 인덱스. |

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

* class [Filter](../../filter/)
* class [FilterCollection](../)
* namespace [Aspose.Tasks](../../filtercollection/)
* assembly [Aspose.Tasks](../../../)


