---
title: "Rsc.PercentWorkComplete"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Rsc 필드. 모든 작업에 대해 완료된 작업의 비율"
type: docs
weight: 550
url: /ko/net/aspose.tasks/rsc/percentworkcomplete/
---
## Rsc.PercentWorkComplete field

모든 작업에 걸쳐 완료된 작업 비율.

```csharp
public static readonly Key<int, RscKey> PercentWorkComplete;
```

## 예제

리소스 작업 완료 비율을 읽는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "ResourcePercentWorkComplete.mpp");

// 모든 리소스에 대한 작업 완료 비율을 표시합니다.
foreach (var res in project.Resources)
{
    if (res.Get(Rsc.Name) != null)
    {
        Console.WriteLine(res.Get(Rsc.PercentWorkComplete));
    }
}
```

### 또 보기

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


