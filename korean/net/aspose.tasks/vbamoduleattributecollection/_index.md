---
title: "클래스 VbaModuleAttributeCollection"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Aspose.Tasks.VbaModuleAttributeCollection 클래스. VbaModuleAttribute 객체의 컬렉션을 나타냅니다."
type: docs
weight: 2830
url: /ko/net/aspose.tasks/vbamoduleattributecollection/
---
## VbaModuleAttributeCollection class

[`VbaModuleAttribute`](../vbamoduleattribute/) 객체의 컬렉션을 나타냅니다.

```csharp
public class VbaModuleAttributeCollection : ReadOnlyCollectionBase<VbaModuleAttribute>
```

## 속성

| 이름 | 설명 |
| --- | --- |
| [Count](../../aspose.tasks/readonlycollectionbase-1/count/) { get; } |  |
| [Item](../../aspose.tasks/readonlycollectionbase-1/item/) { get; set; } |  |

## 메서드

| 이름 | 설명 |
| --- | --- |
| [Add](../../aspose.tasks/readonlycollectionbase-1/add/)(VbaModuleAttribute) |  |
| [GetEnumerator](../../aspose.tasks/readonlycollectionbase-1/getenumerator/)() |  |
| [ToList](../../aspose.tasks/readonlycollectionbase-1/tolist/)() |  |

## 예제

VBA 모듈의 속성 컬렉션을 반복하는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "VbaProject.mpp");

foreach (var module in project.VbaProject.Modules)
{
    Console.WriteLine("Attributes Count: " + module.Attributes.Count);
    foreach (var attribute in module.Attributes)
    {
        Console.WriteLine("Attribute Name: " + attribute.Key);
        Console.WriteLine("Attribute Value: " + attribute.Value);
    }
}
```

### 또 보기

* class [ReadOnlyCollectionBase&lt;T&gt;](../readonlycollectionbase-1/)
* class [VbaModuleAttribute](../vbamoduleattribute/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


