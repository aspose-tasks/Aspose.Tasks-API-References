---
title: "Rsc.IsTeamAssignmentPool"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Rsc 필드. 현재 리소스가 팀 리소스인지 여부를 보여줍니다."
type: docs
weight: 430
url: /ko/net/aspose.tasks/rsc/isteamassignmentpool/
---
## Rsc.IsTeamAssignmentPool field

현재 리소스가 팀 리소스인지 여부를 표시합니다.

```csharp
public static readonly Key<bool, RscKey> IsTeamAssignmentPool;
```

## 예제

Rsc.IsTeamAssignmentPool 속성을 읽고/쓰는 방법을 보여줍니다.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.IsTeamAssignmentPool, true);

Console.WriteLine("Is Team Assignment Pool: " + resource.Get(Rsc.IsTeamAssignmentPool));
```

### 또 보기

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


