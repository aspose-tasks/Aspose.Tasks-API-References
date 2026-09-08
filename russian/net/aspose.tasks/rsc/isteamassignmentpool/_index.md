---
title: "Rsc.IsTeamAssignmentPool"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Rsc field. Показывает, является ли текущий ресурс командным ресурсом"
type: docs
weight: 430
url: /ru/net/aspose.tasks/rsc/isteamassignmentpool/
---
## Rsc.IsTeamAssignmentPool field

Показывает, является ли текущий ресурс командным ресурсом.

```csharp
public static readonly Key<bool, RscKey> IsTeamAssignmentPool;
```

## Примеры

Показывает, как читать/записывать свойство Rsc.IsTeamAssignmentPool.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.IsTeamAssignmentPool, true);

Console.WriteLine("Is Team Assignment Pool: " + resource.Get(Rsc.IsTeamAssignmentPool));
```

### См. также

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


