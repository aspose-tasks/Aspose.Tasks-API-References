---
title: "Rsc.IsBudget"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Rsc 필드. 작업 자재 또는 비용 리소스가 예산 리소스인지 여부를 결정합니다"
type: docs
weight: 380
url: /ko/net/aspose.tasks/rsc/isbudget/
---
## Rsc.IsBudget field

작업, 자재 또는 비용 리소스가 예산 리소스인지 여부를 결정합니다.

```csharp
public static readonly Key<NullableBool, RscKey> IsBudget;
```

## 예제

Rsc.IsBudget 속성을 읽고/쓰는 방법을 보여줍니다.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.IsBudget, true);

Console.WriteLine("Is Budget: " + resource.Get(Rsc.IsBudget));
```

### 또 보기

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


