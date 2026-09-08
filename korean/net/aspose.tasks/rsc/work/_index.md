---
title: "Rsc.Work"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Rsc 필드. 작업에서 리소스에 예정된 총 시간"
type: docs
weight: 690
url: /ko/net/aspose.tasks/rsc/work/
---
## Rsc.Work field

작업에서 리소스에 대해 예정된 총 시간량.

```csharp
public static readonly Key<Duration, RscKey> Work;
```

## 예제

Rsc.Work 속성을 읽고/쓰는 방법을 보여줍니다.

```csharp
var project = new Project();
project.Set(Prj.WorkFormat, TimeUnitType.Day);

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.Work, project.GetWork(1));

Console.WriteLine("Work: " + resource.Get(Rsc.Work));
```

### 또 보기

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


