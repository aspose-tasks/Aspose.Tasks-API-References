---
title: "Rsc.ActualWorkProtected"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Rsc 필드. 실제 작업이 보호되는 작업량"
type: docs
weight: 80
url: /ko/net/aspose.tasks/rsc/actualworkprotected/
---
## Rsc.ActualWorkProtected field

실제 작업이 보호되는 작업량.

```csharp
public static readonly Key<Duration, RscKey> ActualWorkProtected;
```

## 예제

Rsc.ActualWorkProtected 속성을 읽고/쓰는 방법을 보여줍니다.

```csharp
var project = new Project();
project.Set(Prj.WorkFormat, TimeUnitType.Day);

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.ActualWorkProtected, project.GetWork(1));

Console.WriteLine("Actual Work Protected: " + resource.Get(Rsc.ActualWorkProtected));
```

### 또 보기

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


