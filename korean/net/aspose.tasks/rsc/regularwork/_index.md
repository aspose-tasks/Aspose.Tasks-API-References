---
title: "Rsc.RegularWork"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Rsc 필드. 리소스가 수행하도록 예정된 초과 근무가 아닌 작업의 총량"
type: docs
weight: 570
url: /ko/net/aspose.tasks/rsc/regularwork/
---
## Rsc.RegularWork field

리소스가 수행하도록 예정된 비초과 근무의 총량.

```csharp
public static readonly Key<Duration, RscKey> RegularWork;
```

## 예제

Rsc.RegularWork 속성을 읽고/쓰는 방법을 보여줍니다.

```csharp
var project = new Project();
project.Set(Prj.WorkFormat, TimeUnitType.Day);

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.RegularWork, project.GetWork(1));

Console.WriteLine("Regular Work: " + resource.Get(Rsc.RegularWork));
```

### 또 보기

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


