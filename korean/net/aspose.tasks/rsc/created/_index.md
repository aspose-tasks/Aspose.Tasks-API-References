---
title: "Rsc.Created"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Rsc 필드. 리소스가 프로젝트에 추가된 날짜와 시간"
type: docs
weight: 260
url: /ko/net/aspose.tasks/rsc/created/
---
## Rsc.Created field

리소스가 프로젝트에 추가된 날짜와 시간.

```csharp
public static readonly Key<DateTime, RscKey> Created;
```

## 예제

Rsc.Created 속성을 읽고/쓰는 방법을 보여줍니다.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.Created, new DateTime(2020, 4, 10, 8, 0, 0));

Console.WriteLine("Created: " + resource.Get(Rsc.Created));
```

### 또 보기

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


