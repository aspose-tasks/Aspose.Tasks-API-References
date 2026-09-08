---
title: "Rsc.Start"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Rsc 필드. 할당된 리소스가 작업을 시작하도록 예정된 날짜"
type: docs
weight: 640
url: /ko/net/aspose.tasks/rsc/start/
---
## Rsc.Start field

할당된 리소스가 작업을 시작하도록 예정된 날짜.

```csharp
public static readonly Key<DateTime, RscKey> Start;
```

## 예제

Rsc.Start 속성을 읽고 쓰는 방법을 보여줍니다.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.Start, new DateTime(2020, 4, 10, 8, 0, 0));

Console.WriteLine("Start: " + resource.Get(Rsc.Start));
```

### 또 보기

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


