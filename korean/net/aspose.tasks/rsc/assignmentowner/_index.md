---
title: "Rsc.AssignmentOwner"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Rsc 필드. 할당 소유자의 이름"
type: docs
weight: 100
url: /ko/net/aspose.tasks/rsc/assignmentowner/
---
## Rsc.AssignmentOwner field

할당 소유자의 이름.

```csharp
public static readonly Key<string, RscKey> AssignmentOwner;
```

## 예제

Rsc.AssignmentOwner 속성을 읽고/쓰는 방법을 보여줍니다.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.AssignmentOwner, "John");

Console.WriteLine("Assignment Owner: " + resource.Get(Rsc.AssignmentOwner));
```

### 또 보기

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


