---
title: "Prj.CustomDateFormat"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Πεδίο Prj. Προσαρμοσμένη μορφή ημερομηνίας προβολής έργου. Χρησιμοποιείται για τη μορφοποίηση ημερομηνιών όταν η ιδιότητα DateFormat ορίζεται σε Custom."
type: docs
weight: 200
url: /el/net/aspose.tasks/prj/customdateformat/
---
## Prj.CustomDateFormat field

Προσαρμοσμένη μορφή ημερομηνίας προβολής έργου. Χρησιμοποιείται για τη μορφοποίηση ημερομηνιών όταν η ιδιότητα [`DateFormat`](../dateformat/) ορίζεται σε Custom.

```csharp
public static readonly Key<string, PrjKey> CustomDateFormat;
```

## Παραδείγματα

Δείχνει πώς να διαβάσετε/γράψετε την ιδιότητα Prj.CustomDateFormat.

```csharp
var project = new Project();

project.Set(Prj.CustomDateFormat, "dd MMMM yyyy H:mm");

Console.WriteLine("Custom Date Format: " + project.Get(Prj.CustomDateFormat));
```

### Δείτε επίσης

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


