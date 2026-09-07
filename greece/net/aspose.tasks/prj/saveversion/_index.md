---
title: "Prj.SaveVersion"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Πεδίο Prj. Η έκδοση του Microsoft Office Project από την οποία αποθηκεύτηκε ένα αρχείο έργου"
type: docs
weight: 620
url: /el/net/aspose.tasks/prj/saveversion/
---
## Prj.SaveVersion field

Η έκδοση του Microsoft Office Project από την οποία αποθηκεύτηκε ένα αρχείο έργου.

```csharp
public static readonly Key<int, PrjKey> SaveVersion;
```

## Παραδείγματα

Δείχνει πώς να ελέγξετε την έκδοση αποθήκευσης του έργου και την ημερομηνία αποθήκευσης.

```csharp
var project = new Project(DataDir + "DetermineProjectVersion.mpp");

// Εμφάνιση έκδοσης έργου
Console.WriteLine("Project Version : " + project.Get(Prj.SaveVersion));
Console.WriteLine("Last Saved : " + project.Get(Prj.LastSaved).ToShortDateString());
```

### Δείτε επίσης

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


