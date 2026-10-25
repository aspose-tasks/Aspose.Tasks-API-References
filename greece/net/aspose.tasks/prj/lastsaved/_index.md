---
title: "Prj.LastSaved"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Πεδίο Prj. Η ημερομηνία που αποθηκεύτηκε τελευταία φορά το έργο. Αποθηκεύεται σε μορφή UTC σε αρχεία mpp. Τύπος DateTime."
type: docs
weight: 440
url: /el/net/aspose.tasks/prj/lastsaved/
---
## Prj.LastSaved field

Η ημερομηνία κατά την οποία το έργο αποθηκεύτηκε τελευταία φορά. Αποθηκεύεται σε μορφή UTC σε αρχεία mpp. Τύπος DateTime.

```csharp
public static readonly Key<DateTime, PrjKey> LastSaved;
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


