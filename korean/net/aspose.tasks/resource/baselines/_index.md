---
title: "Resource.Baselines"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Resource 속성. 이 객체에 대한 BaselineCollection 인스턴스를 가져옵니다. 리소스의 기준값"
type: docs
weight: 160
url: /ko/net/aspose.tasks/resource/baselines/
---
## Resource.Baselines property

이 객체에 대한 BaselineCollection 인스턴스를 가져옵니다. 리소스의 기준값들입니다.

```csharp
public BaselineCollection Baselines { get; }
```

## 예제

리소스의 기준값을 읽는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "Baselines2010.mpp");

foreach (var resource in project.Resources)
{
    foreach (var baseline in resource.Baselines)
    {
        Console.WriteLine("BaselineNumber: " + baseline.BaselineNumber);
        Console.WriteLine("Bcwp: " + baseline.Bcwp);
        Console.WriteLine("Bcws: " + baseline.Bcws);
        Console.WriteLine("Cost: " + baseline.Cost);
        Console.WriteLine("Work: " + baseline.Work);
    }
}
```

### 또 보기

* class [BaselineCollection](../../baselinecollection/)
* class [Resource](../)
* namespace [Aspose.Tasks](../../resource/)
* assembly [Aspose.Tasks](../../../)


