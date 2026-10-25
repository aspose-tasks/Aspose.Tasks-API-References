---
title: "Rsc.Id"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Rsc 필드. 리소스 목록 내에서 리소스의 위치 식별자"
type: docs
weight: 350
url: /ko/net/aspose.tasks/rsc/id/
---
## Rsc.Id field

리소스 목록 내에서 리소스의 위치 식별자입니다.

```csharp
public static readonly Key<int, RscKey> Id;
```

## 예제

Rsc.Id 속성을 읽고 쓰는 방법을 보여줍니다.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.Id, 987);

Console.WriteLine("Id: " + resource.Get(Rsc.Id));
```

### 또 보기

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


