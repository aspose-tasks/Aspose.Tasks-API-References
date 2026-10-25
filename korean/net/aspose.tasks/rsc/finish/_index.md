---
title: "Rsc.Finish"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Rsc 필드. 리소스가 할당된 모든 작업을 완료하도록 예정된 날짜"
type: docs
weight: 290
url: /ko/net/aspose.tasks/rsc/finish/
---
## Rsc.Finish field

리소스가 할당된 모든 작업을 완료하도록 예정된 날짜.

```csharp
public static readonly Key<DateTime, RscKey> Finish;
```

## 예제

Rsc.Finish 속성을 읽고 쓰는 방법을 보여줍니다.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.Finish, new DateTime(2020, 4, 10, 8, 0, 0));

Console.WriteLine("Finish: " + resource.Get(Rsc.Finish));
```

### 또 보기

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


