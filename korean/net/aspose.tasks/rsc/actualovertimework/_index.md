---
title: "Rsc.ActualOvertimeWork"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Rsc 필드. 작업에 할당된 리소스가 이미 수행한 실제 초과 근무량"
type: docs
weight: 50
url: /ko/net/aspose.tasks/rsc/actualovertimework/
---
## Rsc.ActualOvertimeWork field

작업에 할당된 리소스가 이미 수행한 실제 초과 근무량.

```csharp
public static readonly Key<Duration, RscKey> ActualOvertimeWork;
```

## 예제

Rsc.ActualOvertimeWork 속성을 읽고/쓰는 방법을 보여줍니다.

```csharp
var project = new Project();
project.Set(Prj.WorkFormat, TimeUnitType.Day);

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.ActualOvertimeWork, project.GetWork(1));

Console.WriteLine("Actual Overtime Work: " + resource.Get(Rsc.ActualOvertimeWork));
```

### 또 보기

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


