---
title: "열거형 ItemType"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Aspose.Tasks.ItemType 열거형. 항목의 유형을 지정합니다."
type: docs
weight: 920
url: /ko/net/aspose.tasks/itemtype/
---
## ItemType enumeration

항목의 유형을 지정합니다.

```csharp
public enum ItemType
```

### 값들

| 이름 | 값 | 설명 |
| --- | --- | --- |
| TaskItem | `0` | 작업 항목. |
| ResourceItem | `1` | 리소스 항목. |
| OtherItem | `2` | 기타 항목. |

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


