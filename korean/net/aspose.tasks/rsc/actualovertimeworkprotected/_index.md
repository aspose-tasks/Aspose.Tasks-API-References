---
title: "Rsc.ActualOvertimeWorkProtected"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Rsc 필드. 실제 초과 근무가 보호되는 작업량"
type: docs
weight: 60
url: /ko/net/aspose.tasks/rsc/actualovertimeworkprotected/
---
## Rsc.ActualOvertimeWorkProtected field

실제 초과 근무가 보호되는 작업량.

```csharp
public static readonly Key<Duration, RscKey> ActualOvertimeWorkProtected;
```

## 예제

Rsc.ActualOvertimeWorkProtected 속성을 읽고/쓰는 방법을 보여줍니다.

```csharp
var project = new Project();
project.Set(Prj.WorkFormat, TimeUnitType.Day);

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.ActualOvertimeWorkProtected, project.GetWork(1));

Console.WriteLine("Actual Overtime Work Protected: " + resource.Get(Rsc.ActualOvertimeWorkProtected));
```

### 또 보기

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


