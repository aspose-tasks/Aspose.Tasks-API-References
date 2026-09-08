---
title: "BaselineCollection.Count"
second_title: "Aspose.Tasks for .NET API 참조"
description: "BaselineCollection 속성. 이 BaselineCollection 객체에 포함된 객체 수를 가져옵니다"
type: docs
weight: 10
url: /ko/net/aspose.tasks/baselinecollection/count/
---
## BaselineCollection.Count property

이 BaselineCollection 객체에 포함된 객체 수를 가져옵니다.

```csharp
public int Count { get; }
```

## 예제

Baseline 컬렉션을 사용하는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "WorkWithBaselineCollection.mpp");
var resource = project.Resources.GetByUid(1);

Console.WriteLine("Count of assignment baselines: " + resource.Baselines.Count);
Console.WriteLine("Parent Resource Name: " + resource.Baselines.ParentResource.Get(Rsc.Name));

// Baseline 정보를 읽습니다.
foreach (var baseline in resource.Baselines)
{
    Console.WriteLine("Baseline Number: " + baseline.BaselineNumber);
    Console.WriteLine("Cost: " + baseline.Cost);
    Console.WriteLine("Work: " + baseline.Work);
    Console.WriteLine("BCWP: " + baseline.Bcwp);
    Console.WriteLine("BCWS: " + baseline.Bcws);
    Console.WriteLine();
}

Console.WriteLine("Delete all baselines: ");
List<Baseline> baselines = resource.Baselines.ToList();
foreach (var baseline in baselines)
{
    Console.WriteLine("Delete baseline with name: " + baseline.BaselineNumber);
    resource.Baselines.Remove(baseline);
}
```

### 또 보기

* class [BaselineCollection](../)
* namespace [Aspose.Tasks](../../baselinecollection/)
* assembly [Aspose.Tasks](../../../)


