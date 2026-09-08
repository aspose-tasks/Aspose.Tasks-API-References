---
title: "Asn.Delay"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Asn veld. De vertraging van een toewijzing"
type: docs
weight: 230
url: /nl/net/aspose.tasks/asn/delay/
---
## Asn.Delay field

De vertraging van een opdracht.

```csharp
public static readonly Key<Duration, AsnKey> Delay;
```

## Voorbeelden

Toont hoe je de eigenschappen Asn.Delay en Asn.LevelingDelay kunt lezen/schrijven.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task 1");
task.Set(Tsk.Start, new DateTime(2000, 1, 3, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(8));

var resource = project.Resources.Add("Resource 1");

var assignment = project.ResourceAssignments.Add(task, resource);
assignment.Set(Asn.Delay, project.GetDuration(0, TimeUnitType.Day));

Console.WriteLine("Delay: " + assignment.Get(Asn.Delay));
Console.WriteLine("Leveling Delay: " + assignment.Get(Asn.LevelingDelay));
```

### Zie ook

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


