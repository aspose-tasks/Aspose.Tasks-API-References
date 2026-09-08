---
title: "Filter.ShowInMenu"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Filter 속성. 프로젝트가 리본의 보기 탭에 있는 필터 드롭다운 목록에 필터 이름을 표시할지 여부를 나타내는 값을 가져오거나 설정합니다."
type: docs
weight: 60
url: /ko/net/aspose.tasks/filter/showinmenu/
---
## Filter.ShowInMenu property

리본의 보기 탭에 있는 필터 드롭다운 목록에 프로젝트가 필터 이름을 표시할지 여부를 나타내는 값을 가져오거나 설정합니다.

```csharp
public bool ShowInMenu { get; set; }
```

## 예제

필터를 사용하는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "ReadFilterDefinitionData.mpp");
List<Filter> filters = project.TaskFilters.ToList();
Console.WriteLine("Task filters count: " + filters.Count);
foreach (var filter in filters)
{
    Console.WriteLine("Uid: " + filter.Uid);
    Console.WriteLine("Index: " + filter.Index);
    Console.WriteLine("Name: " + filter.Name);
    Console.WriteLine("Type: " + filter.FilterType);
    Console.WriteLine("Show In Menu: " + filter.ShowInMenu);
    Console.WriteLine("Show Related Summary Rows: " + filter.ShowRelatedSummaryRows);
}

// 리소스 필터 확인
List<Filter> resourceFilters = project.ResourceFilters.ToList();
Console.WriteLine("Project.ResourceFilters count: " + resourceFilters.Count);
Console.WriteLine("Resource Filter Item Type: Item.ResourceType: " + resourceFilters[0].FilterType);
Console.WriteLine("Resource filter ShowInMenu" + resourceFilters[0].ShowInMenu);
Console.WriteLine("Resource filter ShowRelatedSummaryRows: " + resourceFilters[0].ShowRelatedSummaryRows);
```

### 또 보기

* class [Filter](../)
* namespace [Aspose.Tasks](../../filter/)
* assembly [Aspose.Tasks](../../../)


