---
title: "Asn.FixedMaterial"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Asn-veld. Bepaalt of het verbruik van een toegewezen materiaalresource plaatsvindt in één vaste hoeveelheid"
type: docs
weight: 260
url: /nl/net/aspose.tasks/asn/fixedmaterial/
---
## Asn.FixedMaterial field

Bepaalt of het verbruik van een toegewezen materiaalresource plaatsvindt in één vaste hoeveelheid.

```csharp
public static readonly Key<bool, AsnKey> FixedMaterial;
```

## Voorbeelden

Toont hoe de eigenschap Asn.FixedMaterial gelezen/schreven kan worden.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task 1");
task.Set(Tsk.Start, new DateTime(2000, 1, 3, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(8));

var resource = project.Resources.Add("Resource 1");

var assignment = project.ResourceAssignments.Add(task, resource);
assignment.Set(Asn.FixedMaterial, true);

Console.WriteLine("Fixed Material: " + assignment.Get(Asn.FixedMaterial));
```

### Zie ook

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


