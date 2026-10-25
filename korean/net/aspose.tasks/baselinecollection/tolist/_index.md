---
title: "BaselineCollection.ToList"
second_title: "Aspose.Tasks for .NET API 참조"
description: "BaselineCollection 메서드. BaselineCollection 객체를 Baseline 객체 목록으로 변환합니다"
type: docs
weight: 70
url: /ko/net/aspose.tasks/baselinecollection/tolist/
---
## BaselineCollection.ToList method

BaselineCollection 객체를 [`Baseline`](../../baseline/) 객체 목록으로 변환합니다.

```csharp
public List<Baseline> ToList()
```

### 반환 값

[`Baseline`](../../baseline/) 객체 목록.

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

* class [Baseline](../../baseline/)
* class [BaselineCollection](../)
* namespace [Aspose.Tasks](../../baselinecollection/)
* assembly [Aspose.Tasks](../../../)


