---
title: "클래스 Filter"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Aspose.Tasks.Filter 클래스. 프로젝트에서 필터를 나타냅니다"
type: docs
weight: 600
url: /ko/net/aspose.tasks/filter/
---
## Filter class

프로젝트에서 필터를 나타냅니다.

```csharp
public sealed class Filter : IComparable<Filter>, IEquatable<Filter>
```

## 생성자

| 이름 | 설명 |
| --- | --- |
| [Filter](filter/)() | 기본 생성자입니다. |

## 속성

| 이름 | 설명 |
| --- | --- |
| [Criteria](../../aspose.tasks/filter/criteria/) { get; set; } | MSP 보기에서 표시되기 위해 작업 또는 리소스가 충족해야 하는 기준을 가져오거나 설정합니다. |
| [FilterType](../../aspose.tasks/filter/filtertype/) { get; set; } | 필터의 유형을 가져옵니다. |
| [Index](../../aspose.tasks/filter/index/) { get; } | `Filter` 객체가 포함된 Filters 객체에서의 인덱스를 가져옵니다. |
| [Name](../../aspose.tasks/filter/name/) { get; set; } | Filter 객체의 이름을 가져오거나 설정합니다. |
| [ShowInMenu](../../aspose.tasks/filter/showinmenu/) { get; set; } | 리본의 보기 탭에 있는 필터 드롭다운 목록에 프로젝트가 필터 이름을 표시할지 여부를 나타내는 값을 가져오거나 설정합니다. |
| [ShowRelatedSummaryRows](../../aspose.tasks/filter/showrelatedsummaryrows/) { get; set; } | 필터에 대해 관련 요약 행이 표시되는지 여부를 나타내는 값을 가져오거나 설정합니다. |
| [Uid](../../aspose.tasks/filter/uid/) { get; } | 필터의 고유 식별자를 가져옵니다. |

## 메서드

| 이름 | 설명 |
| --- | --- |
| [CompareTo](../../aspose.tasks/filter/compareto/)(Filter) | 이 인스턴스를 지정된 `Filter` 클래스의 인스턴스와 비교하고 상대적인 순서를 나타내는 값을 반환합니다. |
| [Equals](../../aspose.tasks/filter/equals/#equals)(Filter) | 이 인스턴스가 지정된 AssignmentBaseline 객체와 같은지 여부를 나타내는 값을 반환합니다. |
| override [Equals](../../aspose.tasks/filter/equals/#equals_1)(object) | 이 인스턴스가 지정된 AssignmentBaseline 객체와 같은지 여부를 나타내는 값을 반환합니다. |
| override [GetHashCode](../../aspose.tasks/filter/gethashcode/)() | 필터에 대한 해시 코드 값을 반환합니다. |
| [operator ==](../../aspose.tasks/filter/op_equality/) | 이 인스턴스가 지정된 객체와 같은지 여부를 나타내는 값을 반환합니다. |
| [operator &gt;](../../aspose.tasks/filter/op_greaterthan/) | 이 인스턴스가 지정된 객체보다 큰지 여부를 나타내는 값을 반환합니다. |
| [operator &gt;=](../../aspose.tasks/filter/op_greaterthanorequal/) | 이 인스턴스가 지정된 객체보다 크거나 같은지 여부를 나타내는 값을 반환합니다. |
| [operator !=](../../aspose.tasks/filter/op_inequality/) | 이 인스턴스가 지정된 객체와 같지 않은지 여부를 나타내는 값을 반환합니다. |
| [operator &lt;](../../aspose.tasks/filter/op_lessthan/) | 이 인스턴스가 지정된 객체보다 작은지 여부를 나타내는 값을 반환합니다. |
| [operator &lt;=](../../aspose.tasks/filter/op_lessthanorequal/) | 이 인스턴스가 지정된 객체보다 작거나 같은지 여부를 나타내는 값을 반환합니다. |

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


