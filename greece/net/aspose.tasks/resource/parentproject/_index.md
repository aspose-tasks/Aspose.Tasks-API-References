---
title: "Resource.ParentProject"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Ιδιότητα Resource. Λαμβάνει το γονικό έργο για αυτό το κοντέινερ"
type: docs
weight: 600
url: /el/net/aspose.tasks/resource/parentproject/
---
## Resource.ParentProject property

Λαμβάνει το γονικό έργο για αυτό το κοντέινερ.

```csharp
public Project ParentProject { get; }
```

## Παραδείγματα

Δείχνει πώς να χρησιμοποιήσετε το γονικό έργο του πόρου.

```csharp
var project = new Project();
var resource = project.Resources.Add("Resource");

// Ορίστε εργασία για τον πόρο χρησιμοποιώντας τον προεπιλεγμένο τύπο μονάδας χρόνου εργασίας του έργου.
resource.Set(Rsc.Work, resource.ParentProject.GetWork(1));

Console.WriteLine(resource.Get(Rsc.Work));
```

### Δείτε επίσης

* class [Project](../../project/)
* class [Resource](../)
* namespace [Aspose.Tasks](../../resource/)
* assembly [Aspose.Tasks](../../../)


