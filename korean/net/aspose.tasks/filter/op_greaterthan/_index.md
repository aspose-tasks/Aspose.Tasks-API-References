---
title: "Filter.op_GreaterThan"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Filter 메서드. 이 인스턴스가 지정된 객체보다 큰지 여부를 나타내는 값을 반환합니다."
type: docs
weight: 130
url: /ko/net/aspose.tasks/filter/op_greaterthan/
---
## Filter GreaterThan operator

이 인스턴스가 지정된 객체보다 큰지 여부를 나타내는 값을 반환합니다.

```csharp
public static bool operator >(Filter a, Filter b)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| a | Filter | 첫 번째 필터입니다. |
| b | Filter | 두 번째 필터입니다. |

### 반환 값

이 인스턴스가 지정된 객체보다 큰지 여부를 나타내는 값

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


