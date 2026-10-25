---
title: "Prj.WorkFormat"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Πεδίο Prj. Η μορφή που χρησιμοποιείται για την εμφάνιση της διάρκειας της εργασίας"
type: docs
weight: 790
url: /el/net/aspose.tasks/prj/workformat/
---
## Prj.WorkFormat field

Η μορφή που χρησιμοποιείται για την εμφάνιση της διάρκειας της εργασίας.

```csharp
public static readonly Key<TimeUnitType, PrjKey> WorkFormat;
```

## Παραδείγματα

Δείχνει πώς να λάβετε μια διάρκεια με την προεπιλεγμένη μορφή εργασίας.

```csharp
var project = new Project(DataDir + "Blank2010.mpp");

Console.WriteLine("Project's work format: " + project.Get(Prj.WorkFormat));

// δημιουργήστε μια τιμή εργασίας με την προεπιλεγμένη μορφή εργασίας του έργου
var work = project.GetWork(2);
Console.WriteLine("Work: " + work.TimeSpan);
Console.WriteLine("Time unit: " + work.TimeUnit);
```

### Δείτε επίσης

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TimeUnitType](../../timeunittype/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


