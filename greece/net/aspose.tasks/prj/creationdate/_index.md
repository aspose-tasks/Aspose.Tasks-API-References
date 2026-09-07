---
title: "Prj.CreationDate"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Πεδίο Prj. Η ημερομηνία και ώρα δημιουργίας ενός έργου"
type: docs
weight: 130
url: /el/net/aspose.tasks/prj/creationdate/
---
## Prj.CreationDate field

Η ημερομηνία και ώρα κατά τη δημιουργία ενός έργου.

```csharp
public static readonly Key<DateTime, PrjKey> CreationDate;
```

## Παρατηρήσεις

Αποθηκεύεται σε μορφή UTC σε αρχεία mpp. Τύπος DateTime.

## Παραδείγματα

Δείχνει πώς να διαβάσετε/γράψετε την ιδιότητα Prj.CreationDate.

```csharp
var project = new Project();

project.Set(Prj.CreationDate, new DateTime(2020, 4, 10, 8, 0, 0));

Console.WriteLine("Creation Date: " + project.Get(Prj.CreationDate));
```

### Δείτε επίσης

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


