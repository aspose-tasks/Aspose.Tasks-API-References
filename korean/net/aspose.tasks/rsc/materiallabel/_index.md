---
title: "Rsc.MaterialLabel"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Rsc 필드. 물자 리소스의 측정 단위"
type: docs
weight: 440
url: /ko/net/aspose.tasks/rsc/materiallabel/
---
## Rsc.MaterialLabel field

자재 리소스의 측정 단위입니다.

```csharp
public static readonly Key<string, RscKey> MaterialLabel;
```

## 예제

Rsc.MaterialLabel 속성을 읽고 쓰는 방법을 보여줍니다.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.MaterialLabel, "kg");

Console.WriteLine("Material Label: " + resource.Get(Rsc.MaterialLabel));
```

### 또 보기

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


