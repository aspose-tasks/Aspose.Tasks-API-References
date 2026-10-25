---
title: "Rsc.AssignmentOwner"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Πεδίο Rsc. Το όνομα του ιδιοκτήτη ανάθεσης."
type: docs
weight: 100
url: /el/net/aspose.tasks/rsc/assignmentowner/
---
## Rsc.AssignmentOwner field

Το όνομα του ιδιοκτήτη ανάθεσης.

```csharp
public static readonly Key<string, RscKey> AssignmentOwner;
```

## Παραδείγματα

Δείχνει πώς να διαβάσετε/γράψετε την ιδιότητα Rsc.AssignmentOwner.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.AssignmentOwner, "John");

Console.WriteLine("Assignment Owner: " + resource.Get(Rsc.AssignmentOwner));
```

### Δείτε επίσης

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


