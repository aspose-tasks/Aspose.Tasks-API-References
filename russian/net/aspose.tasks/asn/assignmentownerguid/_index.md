---
title: "Asn.AssignmentOwnerGuid"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Поле Asn. Глобальный уникальный идентификатор владельца назначения"
type: docs
weight: 110
url: /ru/net/aspose.tasks/asn/assignmentownerguid/
---
## Asn.AssignmentOwnerGuid field

Глобальный уникальный идентификатор владельца назначения.

```csharp
public static readonly Key<string, AsnKey> AssignmentOwnerGuid;
```

## Примеры

Показывает, как читать/записывать свойства Asn.AssignmentOwner и Asn.AssignmentOwnerGuid.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task 1");
task.Set(Tsk.Start, new DateTime(2000, 1, 3, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(8));

var resource = project.Resources.Add("Resource 1");
resource.Set(Rsc.Type, ResourceType.Work);

var assignment = project.ResourceAssignments.Add(task, resource);
assignment.Set(Asn.AssignmentOwner, "Assignment Owner");
assignment.Set(Asn.AssignmentOwnerGuid, "1d440f0c-7839-4802-af5f-4bb30e8b75ab");

Console.WriteLine("Assignment Owner: " + assignment.Get(Asn.AssignmentOwner));
Console.WriteLine("Assignment Owner GUID: " + assignment.Get(Asn.AssignmentOwnerGuid));
```

### См. также

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


