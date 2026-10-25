---
title: "Rsc.Uid"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Rsc 필드. 리소스의 고유 식별자"
type: docs
weight: 670
url: /ko/net/aspose.tasks/rsc/uid/
---
## Rsc.Uid field

리소스의 고유 식별자.

```csharp
public static readonly Key<int, RscKey> Uid;
```

## 예제

Rsc.Uid 속성을 읽고 쓰는 방법을 보여줍니다.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.Uid, 99);

Console.WriteLine("Uid: " + resource.Get(Rsc.Uid));
```

### 또 보기

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


