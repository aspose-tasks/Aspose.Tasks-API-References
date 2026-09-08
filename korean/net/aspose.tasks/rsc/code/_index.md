---
title: "Rsc.Code"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Rsc 필드. 리소스에 대한 코드 또는 기타 정보"
type: docs
weight: 210
url: /ko/net/aspose.tasks/rsc/code/
---
## Rsc.Code field

리소스에 대한 코드 또는 기타 정보.

```csharp
public static readonly Key<string, RscKey> Code;
```

## 예제

Rsc.Code 속성을 읽고/쓰는 방법을 보여줍니다.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.Code, "555292");

Console.WriteLine("Code: " + resource.Get(Rsc.Code));
```

### 또 보기

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


