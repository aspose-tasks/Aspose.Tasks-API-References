---
title: "Rsc.Name"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Rsc 필드. 리소스의 이름"
type: docs
weight: 460
url: /ko/net/aspose.tasks/rsc/name/
---
## Rsc.Name field

리소스의 이름입니다.

```csharp
public static readonly Key<string, RscKey> Name;
```

## 예제

Rsc.Name 속성을 읽고 쓰는 방법을 보여줍니다.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.Name, "John Smith");

Console.WriteLine("Name: " + resource.Get(Rsc.Name));
```

### 또 보기

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


