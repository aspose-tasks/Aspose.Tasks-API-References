---
title: "Κλάση VbaModule"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Κλάση Aspose.Tasks.VbaModule. Αντιπροσωπεύει μια μονάδα VBA"
type: docs
weight: 2810
url: /el/net/aspose.tasks/vbamodule/
---
## VbaModule class

Αντιπροσωπεύει ένα μονάδα VBA.

```csharp
public sealed class VbaModule
```

## Ιδιότητες

| Όνομα | Περιγραφή |
| --- | --- |
| [Attributes](../../aspose.tasks/vbamodule/attributes/) { get; } | Λαμβάνει μια συλλογή των χαρακτηριστικών της μονάδας. |
| [Name](../../aspose.tasks/vbamodule/name/) { get; set; } | Λαμβάνει ένα όνομα της μονάδας VBA |
| [SourceCode](../../aspose.tasks/vbamodule/sourcecode/) { get; set; } | Λαμβάνει ή ορίζει τον πηγαίο κώδικα της μονάδας VBA |
| [Type](../../aspose.tasks/vbamodule/type/) { get; } | Λαμβάνει τον τύπο της μονάδας. |

## Μέθοδοι

| Όνομα | Περιγραφή |
| --- | --- |
| static [CreateClassModule](../../aspose.tasks/vbamodule/createclassmodule/)(string) | Δημιουργεί μια παρουσία της `VbaModule` με τύπο VbaModuleType.ClassModule. |
| static [CreateProceduralModule](../../aspose.tasks/vbamodule/createproceduralmodule/)(string) | Δημιουργεί μια παρουσία της `VbaModule` με τύπο VbaModuleType.ProceduralModule. |

## Παραδείγματα

Δείχνει πώς να διαβάσετε τις μονάδες του έργου VBA.

```csharp
var project = new Project(DataDir + "VbaProject.mpp");

Console.WriteLine("Total Modules Count: " + project.VbaProject.Modules.Count);

foreach (var module in project.VbaProject.Modules)
{
    Console.WriteLine("Module Name: " + module.Name);
    Console.WriteLine("Source Code: " + module.SourceCode);
}
```

### Δείτε επίσης

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


