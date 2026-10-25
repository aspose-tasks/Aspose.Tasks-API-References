---
title: "Rsc.AssignmentOwner"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Поле Rsc. Имя владельца назначения"
type: docs
weight: 100
url: /ru/net/aspose.tasks/rsc/assignmentowner/
---
## Rsc.AssignmentOwner field

Имя владельца назначения.

```csharp
public static readonly Key<string, RscKey> AssignmentOwner;
```

## Примеры

Показывает, как читать/записывать свойство Rsc.AssignmentOwner.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.AssignmentOwner, "John");

Console.WriteLine("Assignment Owner: " + resource.Get(Rsc.AssignmentOwner));
```

### См. также

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


