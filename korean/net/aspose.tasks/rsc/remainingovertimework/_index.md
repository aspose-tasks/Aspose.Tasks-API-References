---
title: "Rsc.RemainingOvertimeWork"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Rsc 필드. 남은 예정 초과 근무량"
type: docs
weight: 600
url: /ko/net/aspose.tasks/rsc/remainingovertimework/
---
## Rsc.RemainingOvertimeWork field

남은 예정 초과 근무량.

```csharp
public static readonly Key<Duration, RscKey> RemainingOvertimeWork;
```

## 예제

Rsc.RemainingOvertimeWork 속성을 읽고/쓰는 방법을 보여줍니다.

```csharp
var project = new Project();
project.Set(Prj.WorkFormat, TimeUnitType.Day);

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.RemainingOvertimeWork, project.GetWork(1));

Console.WriteLine("Remaining Overtime Work: " + resource.Get(Rsc.RemainingOvertimeWork));
```

### 또 보기

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


