---
title: "Gridline.GetHashCode"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Gridline 메서드. Gridline 클래스 인스턴스에 대한 해시 코드 값을 반환합니다."
type: docs
weight: 60
url: /ko/net/aspose.tasks.visualization/gridline/gethashcode/
---
## Gridline.GetHashCode method

`[`Gridline`](../) 클래스` 인스턴스에 대한 해시 코드 값을 반환합니다.

```csharp
public override int GetHashCode()
```

### 반환 값

이 객체에 대한 해시 코드 값을 반환합니다.

## 예제

그리드라인의 해시 코드를 가져오는 방법을 보여줍니다.

```csharp
var gridline1 = new Gridline();
var gridline2 = new Gridline();

// 그리드라인의 해시 코드는 내부 GUID 필드를 기반으로 합니다.
Console.WriteLine("Gridline 1 Hash Code: {0}", gridline1.GetHashCode());
Console.WriteLine("Gridline 2 Hash Code: {0}", gridline2.GetHashCode());
```

### 또 보기

* class [Gridline](../)
* namespace [Aspose.Tasks.Visualization](../../gridline/)
* assembly [Aspose.Tasks](../../../)


