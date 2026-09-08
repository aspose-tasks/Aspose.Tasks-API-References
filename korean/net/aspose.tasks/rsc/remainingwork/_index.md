---
title: "Rsc.RemainingWork"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Rsc 필드. 작업 또는 작업 집합을 완료하는 데 아직 필요한 시간"
type: docs
weight: 610
url: /ko/net/aspose.tasks/rsc/remainingwork/
---
## Rsc.RemainingWork field

작업 또는 작업 집합을 완료하는 데 아직 필요한 시간.

```csharp
public static readonly Key<Duration, RscKey> RemainingWork;
```

## 예제

Rsc.RemainingWork 속성을 읽고/쓰는 방법을 보여줍니다.

```csharp
var project = new Project();
project.Set(Prj.WorkFormat, TimeUnitType.Day);

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.RemainingWork, project.GetWork(1));

Console.WriteLine("Remaining Work: " + resource.Get(Rsc.RemainingWork));
```

### 또 보기

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


