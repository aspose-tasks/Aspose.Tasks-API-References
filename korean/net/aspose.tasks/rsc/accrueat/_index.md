---
title: "Rsc.AccrueAt"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Rsc 필드. 리소스 표준 및 초과 근무 비용이 작업 비용에 언제, 어떻게 청구되거나 발생되는지를 결정합니다."
type: docs
weight: 10
url: /ko/net/aspose.tasks/rsc/accrueat/
---
## Rsc.AccrueAt field

리소스 표준 및 초과 근무 비용이 작업 비용에 청구되거나 발생되는 시점과 방식을 결정합니다.

```csharp
public static readonly Key<CostAccrualType, RscKey> AccrueAt;
```

## 예제

Rsc.AccrueAt 속성을 읽고/쓰는 방법을 보여줍니다.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.AccrueAt, CostAccrualType.End);

Console.WriteLine("Accrue At: " + resource.Get(Rsc.AccrueAt));
```

### 또 보기

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [CostAccrualType](../../costaccrualtype/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


