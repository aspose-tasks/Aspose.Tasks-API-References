---
title: "Rsc.AssignmentOwnerGuid"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Rsc 필드. 할당 소유자의 GUID"
type: docs
weight: 110
url: /ko/net/aspose.tasks/rsc/assignmentownerguid/
---
## Rsc.AssignmentOwnerGuid field

할당 소유자의 GUID.

```csharp
public static readonly Key<string, RscKey> AssignmentOwnerGuid;
```

## 예제

Rsc.AssignmentOwnerGuid 속성을 읽고/쓰는 방법을 보여줍니다.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.AssignmentOwnerGuid, "aad9ac22-9f06-4196-906b-916acebcc1c2");

Console.WriteLine("Assignment Owner Guid: " + resource.Get(Rsc.AssignmentOwnerGuid));
```

### 또 보기

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


