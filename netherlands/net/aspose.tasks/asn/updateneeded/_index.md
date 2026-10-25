---
title: "Asn.UpdateNeeded"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Asn-veld. Bepaalt of de aan een taak toegewezen resource moet worden bijgewerkt met betrekking tot de status van de taak"
type: docs
weight: 580
url: /nl/net/aspose.tasks/asn/updateneeded/
---
## Asn.UpdateNeeded field

Bepaalt of de aan een taak toegewezen resource moet worden bijgewerkt met betrekking tot de status van de taak.

```csharp
public static readonly Key<bool, AsnKey> UpdateNeeded;
```

## Voorbeelden

Toont hoe de eigenschap Asn.UpdateNeeded te lezen/schrijven.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task 1");
task.Set(Tsk.Start, new DateTime(2000, 1, 3, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(8));

var resource = project.Resources.Add("Resource 1");

var assignment = project.ResourceAssignments.Add(task, resource);
assignment.Set(Asn.UpdateNeeded, true);

Console.WriteLine("Update Needed: " + assignment.Get(Asn.UpdateNeeded));
```

### Zie ook

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


