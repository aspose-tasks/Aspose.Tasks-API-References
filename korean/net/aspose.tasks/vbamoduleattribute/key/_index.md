---
title: "VbaModuleAttribute.Key"
second_title: "Aspose.Tasks for .NET API 참조"
description: "VbaModuleAttribute 속성. VBA 모듈 속성의 키를 가져옵니다"
type: docs
weight: 10
url: /ko/net/aspose.tasks/vbamoduleattribute/key/
---
## VbaModuleAttribute.Key property

VBA 모듈 속성의 키를 가져옵니다.

```csharp
public string Key { get; }
```

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

* class [VbaModuleAttribute](../)
* namespace [Aspose.Tasks](../../vbamoduleattribute/)
* assembly [Aspose.Tasks](../../../)


