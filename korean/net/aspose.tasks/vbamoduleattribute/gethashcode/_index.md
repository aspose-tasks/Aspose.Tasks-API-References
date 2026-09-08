---
title: "VbaModuleAttribute.GetHashCode"
second_title: "Aspose.Tasks for .NET API 참조"
description: "VbaModuleAttribute 메서드. 이 VbaModuleAttribute에 대한 해시 코드 값을 반환합니다."
type: docs
weight: 40
url: /ko/net/aspose.tasks/vbamoduleattribute/gethashcode/
---
## VbaModuleAttribute.GetHashCode method

이 [`VbaModuleAttribute`](../)에 대한 해시 코드 값을 반환합니다.

```csharp
public override int GetHashCode()
```

### 반환 값

이 객체에 대한 해시 코드 값을 반환합니다.

## 예제

VBA 모듈 속성의 해시 코드를 얻는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "VbaProject.mpp");
var module = project.VbaProject.Modules.ToList()[0];

var attribute1 = module.Attributes.ToList()[0];
var attribute2 = module.Attributes.ToList()[0];

// VBA 모듈 속성들의 해시 코드를 출력합니다
Console.WriteLine("Hash codes of VBA module attributes are based on key and value hash codes.");
Console.WriteLine("VBA module attribute 1 Hash Code: {0}", attribute1.GetHashCode());
Console.WriteLine("VBA module attribute 2 Hash Code: {0}", attribute2.GetHashCode());
```

### 또 보기

* class [VbaModuleAttribute](../)
* namespace [Aspose.Tasks](../../vbamoduleattribute/)
* assembly [Aspose.Tasks](../../../)


