---
title: "Rsc.ActualWork"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Rsc 필드. 작업에 할당된 리소스가 이미 수행한 작업량"
type: docs
weight: 70
url: /ko/net/aspose.tasks/rsc/actualwork/
---
## Rsc.ActualWork field

작업에 할당된 리소스가 이미 수행한 작업량.

```csharp
public static readonly Key<Duration, RscKey> ActualWork;
```

## 예제

Rsc.ActualWork 속성을 읽고 쓰는 방법을 보여줍니다.

```csharp
var project = new Project();
project.Set(Prj.WorkFormat, TimeUnitType.Day);

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.ActualWork, project.GetWork(1));

Console.WriteLine("Actual Work: " + resource.Get(Rsc.ActualWork));
```

### 또 보기

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


