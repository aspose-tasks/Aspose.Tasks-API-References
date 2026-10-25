---
title: "Rsc.AssignmentOwnerGuid"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Поле Rsc. GUID владельца назначения"
type: docs
weight: 110
url: /ru/net/aspose.tasks/rsc/assignmentownerguid/
---
## Rsc.AssignmentOwnerGuid field

GUID владельца назначения.

```csharp
public static readonly Key<string, RscKey> AssignmentOwnerGuid;
```

## Примеры

Показывает, как читать/записывать свойство Rsc.AssignmentOwnerGuid.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.AssignmentOwnerGuid, "aad9ac22-9f06-4196-906b-916acebcc1c2");

Console.WriteLine("Assignment Owner Guid: " + resource.Get(Rsc.AssignmentOwnerGuid));
```

### См. также

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


