---
title: "Rsc.IsEnterprise"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Rsc 필드. 리소스가 엔터프라이즈 리소스 풀에 속하는지(true) 혹은 로컬 리소스 풀에 속하는지(false)를 표시합니다"
type: docs
weight: 400
url: /ko/net/aspose.tasks/rsc/isenterprise/
---
## Rsc.IsEnterprise field

리소스가 기업 리소스 풀에 속하는지(true) 혹은 로컬 리소스 풀에 속하는지(false)를 표시합니다.

```csharp
public static readonly Key<NullableBool, RscKey> IsEnterprise;
```

## 예제

Rsc.IsEnterprise 속성을 읽고/쓰는 방법을 보여줍니다.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.IsEnterprise, true);

Console.WriteLine("Is Enterprise: " + resource.Get(Rsc.IsEnterprise));
```

### 또 보기

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


