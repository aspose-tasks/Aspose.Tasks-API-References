---
title: "Κλάση VbaProject"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Aspose.Tasks.VbaProject κλάση. Αντιπροσωπεύει το VbaProject"
type: docs
weight: 2860
url: /el/net/aspose.tasks/vbaproject/
---
## VbaProject class

Αντιπροσωπεύει το `VbaProject`.

```csharp
public class VbaProject
```

## Ιδιότητες

| Όνομα | Περιγραφή |
| --- | --- |
| [CompilationArguments](../../aspose.tasks/vbaproject/compilationarguments/) { get; } | Λαμβάνει τα ορίσματα συνθήκης μεταγλώττισης |
| [Description](../../aspose.tasks/vbaproject/description/) { get; } | Λαμβάνει μια περιγραφή του έργου. |
| [HelpContextId](../../aspose.tasks/vbaproject/helpcontextid/) { get; } | Λαμβάνει το Id περιβάλλοντος βοήθειας του έργου |
| [HelpFile](../../aspose.tasks/vbaproject/helpfile/) { get; } | Λαμβάνει το όνομα του αρχείου βοήθειας |
| [Modules](../../aspose.tasks/vbaproject/modules/) { get; } | Λαμβάνει μια συλλογή από [`VbaModuleCollection`](../vbamodulecollection/) |
| [Name](../../aspose.tasks/vbaproject/name/) { get; } | Λαμβάνει το όνομα του έργου |
| [References](../../aspose.tasks/vbaproject/references/) { get; } | Λαμβάνει μια συλλογή από [`VbaReferenceCollection`](../vbareferencecollection/) |

## Παραδείγματα

Δείχνει πώς να διαβάσετε τις ιδιότητες του έργου VBA.

```csharp
var project = new Project(DataDir + "VbaProject.mpp");

Console.WriteLine("VbaProject.Name " + project.VbaProject.Name);
Console.WriteLine("VbaProject.Description " + project.VbaProject.Description);
Console.WriteLine("VbaProject.CompilationArguments" + project.VbaProject.CompilationArguments);
Console.WriteLine("VbaProject.HelpContextId" + project.VbaProject.HelpContextId);
Console.WriteLine("VbaProject.HelpFile" + project.VbaProject.HelpFile);
```

### Δείτε επίσης

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


