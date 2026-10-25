---
title: "Rsc.Workgroup"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Rsc 필드. 리소스가 속한 작업 그룹의 유형"
type: docs
weight: 700
url: /ko/net/aspose.tasks/rsc/workgroup/
---
## Rsc.Workgroup field

리소스가 속한 작업 그룹 유형.

```csharp
public static readonly Key<WorkGroupType, RscKey> Workgroup;
```

## 예제

Rsc.Workgroup 속성을 읽고/쓰는 방법을 보여줍니다.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.Workgroup, WorkGroupType.Email);

Console.WriteLine("Workgroup: " + resource.Get(Rsc.Workgroup));
```

### 또 보기

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [WorkGroupType](../../workgrouptype/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


