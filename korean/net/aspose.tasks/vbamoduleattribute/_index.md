---
title: "클래스 VbaModuleAttribute"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Aspose.Tasks.VbaModuleAttribute 클래스. VbaModule 객체의 속성입니다."
type: docs
weight: 2820
url: /ko/net/aspose.tasks/vbamoduleattribute/
---
## VbaModuleAttribute class

[`VbaModule`](../vbamodule/) 객체의 속성입니다.

```csharp
public sealed class VbaModuleAttribute : IEquatable<VbaModuleAttribute>
```

## 속성

| 이름 | 설명 |
| --- | --- |
| [Key](../../aspose.tasks/vbamoduleattribute/key/) { get; } | VBA 모듈 속성의 키를 가져옵니다. |
| [Value](../../aspose.tasks/vbamoduleattribute/value/) { get; } | VBA 모듈 속성의 값을 가져옵니다. |

## 메서드

| 이름 | 설명 |
| --- | --- |
| override [Equals](../../aspose.tasks/vbamoduleattribute/equals/#equals_1)(object) | 이 인스턴스가 지정된 `VbaModuleAttribute` 객체와 같은지 여부를 나타내는 값을 반환합니다. |
| [Equals](../../aspose.tasks/vbamoduleattribute/equals/#equals)(VbaModuleAttribute) | 이 인스턴스가 지정된 `VbaModuleAttribute` 객체와 같은지 여부를 나타내는 값을 반환합니다. |
| override [GetHashCode](../../aspose.tasks/vbamoduleattribute/gethashcode/)() | 이 `VbaModuleAttribute`에 대한 해시 코드 값을 반환합니다. |

## 예제

VBA 모듈 속성을 사용하는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "VbaProject.mpp");

foreach (var module in project.VbaProject.Modules)
{
    Console.WriteLine("Attributes Count: " + module.Attributes.Count);
    foreach (var attribute in module.Attributes)
    {
        Console.WriteLine("  VB Name: " + attribute.Key);
        Console.WriteLine("  Module: " + attribute.Value);
    }
}
```

### 또 보기

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


