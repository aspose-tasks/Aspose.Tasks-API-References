---
title: "IVbaModule.Attributes"
second_title: "Aspose.Tasks for .NET API 참조"
description: "IVbaModule 속성. VbaModuleAttributeCollection 컬렉션을 가져옵니다."
type: docs
weight: 10
url: /ko/net/aspose.tasks/ivbamodule/attributes/
---
## IVbaModule.Attributes property

`[`VbaModuleAttributeCollection`](../../vbamoduleattributecollection/)` 컬렉션을 가져옵니다.

```csharp
public VbaModuleAttributeCollection Attributes { get; }
```

## 예제

VBA 모듈의 속성을 읽는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "VbaProject.mpp");

foreach (var module in project.VbaProject.Modules)
{
    Console.WriteLine("Attributes Count: " + module.Attributes.Count);
    foreach (var attribute in module.Attributes)
    {
        Console.WriteLine("VB Name: " + attribute.Key);
        Console.WriteLine("Module: " + attribute.Value);
    }
}
```

### 또 보기

* class [VbaModuleAttributeCollection](../../vbamoduleattributecollection/)
* interface [IVbaModule](../)
* namespace [Aspose.Tasks](../../ivbamodule/)
* assembly [Aspose.Tasks](../../../)


