---
title: "Rsc.IsTeamAssignmentPool"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Rsc 字段。显示当前资源是否为团队资源"
type: docs
weight: 430
url: /zh/net/aspose.tasks/rsc/isteamassignmentpool/
---
## Rsc.IsTeamAssignmentPool field

显示当前资源是否为团队资源。

```csharp
public static readonly Key<bool, RscKey> IsTeamAssignmentPool;
```

## 示例

展示如何读取/写入 Rsc.IsTeamAssignmentPool 属性。

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.IsTeamAssignmentPool, true);

Console.WriteLine("Is Team Assignment Pool: " + resource.Get(Rsc.IsTeamAssignmentPool));
```

### 另见

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


