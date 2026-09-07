---
title: "Prj.LastPrinted"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Πεδίο Prj. Τελευταία ώρα εκτύπωσης του έργου. Αποθηκεύεται σε μορφή UTC σε αρχεία mpp. Τύπος DateTime."
type: docs
weight: 430
url: /el/net/aspose.tasks/prj/lastprinted/
---
## Prj.LastPrinted field

Τελευταία ώρα εκτύπωσης του έργου. Αποθηκεύεται σε μορφή UTC σε αρχεία mpp. Τύπος DateTime.

```csharp
public static readonly Key<DateTime, PrjKey> LastPrinted;
```

## Παραδείγματα

Δείχνει πώς να διαβάσετε/γράψετε την ιδιότητα Prj.LastPrinted.

```csharp
var project = new Project();

project.Set(Prj.LastPrinted, new DateTime(2020, 4, 10, 13, 0, 0));

Console.WriteLine("Last Printed: " + project.Get(Prj.LastPrinted));
```

### Δείτε επίσης

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


