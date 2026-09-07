---
title: "Prj.ExtendedCreationDate"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Prj πεδίο. Η ημερομηνία που χρησιμοποιείται για υπολογισμό και αναφορά"
type: docs
weight: 320
url: /el/net/aspose.tasks/prj/extendedcreationdate/
---
## Prj.ExtendedCreationDate field

Ημερομηνία που χρησιμοποιείται για υπολογισμό και αναφορά.

```csharp
public static readonly Key<DateTime, PrjKey> ExtendedCreationDate;
```

## Παραδείγματα

Δείχνει πώς να διαβάσετε/γράψετε την ιδιότητα Prj.ExtendedCreationDate.

```csharp
var project = new Project();

project.Set(Prj.ExtendedCreationDate, new DateTime(2020, 4, 10, 9, 0, 0));

Console.WriteLine("Extended Creation Date: " + project.Get(Prj.ExtendedCreationDate));
```

### Δείτε επίσης

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


