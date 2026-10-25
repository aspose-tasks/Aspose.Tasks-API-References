---
title: "Δομή KeyTK"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Δομή Aspose.Tasks.Key2TK. Αναπαριστά ένα κλειδί ιδιότητας μιας κλάσης του καθορισμένου τύπου. Μια παρουσία αυτής της κλάσης χρησιμοποιείται κατά τη λήψη ή τον ορισμό ιδιότητας ενός περιέκτη."
type: docs
weight: 930
url: /el/net/aspose.tasks/key-2/
---
## Key&lt;T,K&gt; structure

Αναπαριστά ένα κλειδί ιδιότητας μιας κλάσης του καθορισμένου τύπου. Μια παρουσία αυτής της κλάσης χρησιμοποιείται όταν λαμβάνεται ή ορίζεται η ιδιότητα ενός δοχείου.

```csharp
public struct Key<T, K>
    where K : struct
```

| Παράμετρος | Περιγραφή |
| --- | --- |
| T | Ο τύπος της τιμής ιδιότητας. |
| K | Ο τύπος του κλειδιού ιδιότητας. |

## Ιδιότητες

| Όνομα | Περιγραφή |
| --- | --- |
| [KeyType](../../aspose.tasks/key-2/keytype/) { get; } | Λαμβάνει το κλειδί της ιδιότητας. |

## Παραδείγματα

Δείχνει πώς να διαβάσετε/γράψετε την ιδιότητα Prj.ActualsInSync.

```csharp
var project = new Project();

project.Set(Prj.ActualsInSync, true);

Console.WriteLine("Actuals In Sync: " + project.Get(Prj.ActualsInSync));
```

### Δείτε επίσης

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


