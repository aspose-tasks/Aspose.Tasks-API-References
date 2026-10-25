---
title: "Gridline.Equals"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Gridline 메서드. 이 인스턴스가 지정된 객체와 같은지 여부를 나타내는 플래그를 반환합니다."
type: docs
weight: 50
url: /ko/net/aspose.tasks.visualization/gridline/equals/
---
## Gridline.Equals method

이 인스턴스가 지정된 객체와 같은지 여부를 나타내는 플래그를 반환합니다.

```csharp
public override bool Equals(object obj)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| obj | Object | 이 인스턴스와 비교할 지정된 객체. |

### 반환 값

이 인스턴스가 지정된 객체와 같은지 여부를 나타내는 플래그.

## 예제

그리드선의 동일성을 확인하는 방법을 보여줍니다.

```csharp
var gridline1 = new Gridline();
var gridline2 = new Gridline();

// 그리드선의 동일성은 그리드선 유형에 대해 확인됩니다.
Console.WriteLine("Gridline 1 Type: " + gridline1.GridlineType);
Console.WriteLine("Gridline 2 Type: " + gridline2.GridlineType);
Console.WriteLine("Are gridlines equal: " + gridline1.Equals(gridline2));

// 유형을 변경합니다.
gridline1.GridlineType = GridlineType.BarRows;
Console.WriteLine("Gridline 1 Type: " + gridline1.GridlineType);
Console.WriteLine("Are gridlines equal: " + gridline1.Equals(gridline2));
```

### 또 보기

* class [Gridline](../)
* namespace [Aspose.Tasks.Visualization](../../gridline/)
* assembly [Aspose.Tasks](../../../)


