---
title: "Prj.StatusDate"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Πεδίο Prj. Η ημερομηνία κατάστασης για την εμφάνιση προόδου ή για τον υπολογισμό συνολικών κερδών αξίας. Η ημερομηνία κατάστασης είναι η ίδια με την τρέχουσα ημερομηνία, εκτός εάν καθοριστεί διαφορετική ημερομηνία κατάστασης."
type: docs
weight: 690
url: /el/net/aspose.tasks/prj/statusdate/
---
## Prj.StatusDate field

η ημερομηνία κατάστασης για την εμφάνιση προόδου ή για τον υπολογισμό των συνολικών κερδισμένων αξιών. Η ημερομηνία κατάστασης είναι η ίδια με την τρέχουσα ημερομηνία (η σημερινή ημερομηνία) εκτός εάν καθοριστεί διαφορετική ημερομηνία κατάστασης.

```csharp
public static readonly Key<DateTime, PrjKey> StatusDate;
```

## Παραδείγματα

Δείχνει πώς να διαβάσετε/γράψετε την ιδιότητα Prj.StatusDate.

```csharp
var project = new Project();

project.Set(Prj.StatusDate, new DateTime(2020, 4, 19, 8, 0, 0));

Console.WriteLine("Status Date: " + project.Get(Prj.StatusDate));
```

### Δείτε επίσης

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


