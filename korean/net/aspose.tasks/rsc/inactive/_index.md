---
title: "Rsc.Inactive"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Rsc 필드. 관리 권한을 가진 사용자가 리소스를 비활성화했는지 여부를 결정합니다"
type: docs
weight: 360
url: /ko/net/aspose.tasks/rsc/inactive/
---
## Rsc.Inactive field

관리자 권한을 가진 사용자가 리소스를 비활성화했는지 여부를 결정합니다.

```csharp
public static readonly Key<NullableBool, RscKey> Inactive;
```

## 예제

Rsc.Inactive 속성을 읽고/쓰는 방법을 보여줍니다.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.Inactive, true);

Console.WriteLine("Inactive: " + resource.Get(Rsc.Inactive));
```

### 또 보기

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


