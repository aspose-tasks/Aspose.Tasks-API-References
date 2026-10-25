---
title: "Filter.CompareTo"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Filter 메서드. 이 인스턴스를 지정된 Filter 클래스 인스턴스와 비교하고 상대 순서에 대한 표시를 반환합니다."
type: docs
weight: 90
url: /ko/net/aspose.tasks/filter/compareto/
---
## Filter.CompareTo method

이 인스턴스를 [`Filter`](../) 클래스의 지정된 인스턴스와 비교하고 상대 순서에 대한 표시를 반환합니다.

```csharp
public int CompareTo(Filter other)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| other | Filter | 이 객체와 비교할 [`Filter`](../) 클래스의 지정된 인스턴스. |

### 반환 값

그들의 상대 순서에 대한 표시.

## 예제

필터 동등성을 확인하는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "ReadFilterDefinitionData.mpp");
List<Filter> filters = project.TaskFilters.ToList();

var filter1 = filters[0];
var filter2 = filters[1];

// 필터의 동등성은 필터 UID와 비교하여 확인됩니다.
Console.WriteLine("Filter 1 UID: " + filter1.Uid);
Console.WriteLine("Filter 2 UID: " + filter2.Uid);
Console.WriteLine("Are filters equal: " + filter1.Equals(filter2));
```

### 또 보기

* class [Filter](../)
* namespace [Aspose.Tasks](../../filter/)
* assembly [Aspose.Tasks](../../../)


