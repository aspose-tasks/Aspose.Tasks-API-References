---
title: "Rsc.Initials"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Rsc 필드. 리소스의 이니셜"
type: docs
weight: 370
url: /ko/net/aspose.tasks/rsc/initials/
---
## Rsc.Initials field

리소스의 이니셜입니다.

```csharp
public static readonly Key<string, RscKey> Initials;
```

## 예제

Rsc.Initials 속성을 읽고 쓰는 방법을 보여줍니다.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.Initials, "R");

Console.WriteLine("Initials: " + resource.Get(Rsc.Initials));
```

### 또 보기

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


