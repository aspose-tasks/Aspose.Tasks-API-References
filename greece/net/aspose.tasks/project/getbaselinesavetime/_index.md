---
title: "Project.GetBaselineSaveTime"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Μέθοδος Project. Επιστρέφει το χρόνο αποθήκευσης της βάσης"
type: docs
weight: 1090
url: /el/net/aspose.tasks/project/getbaselinesavetime/
---
## Project.GetBaselineSaveTime method

Επιστρέφει τον χρόνο αποθήκευσης της βάσης.

```csharp
public DateTime GetBaselineSaveTime(BaselineType baselineNumber)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| baselineNumber | BaselineType | Ο αριθμός του baseline [`BaselineType`](../../baselinetype/). |

### Τιμή Επιστροφής

Η τελευταία ημερομηνία και ώρα αποθήκευσης του baseline.

## Παρατηρήσεις

Επιστρέφει DateTime.MinValue εάν η βάση δεν αποθηκεύτηκε.

## Παραδείγματα

Δείχνει πώς να διαβάσετε/γράψετε το χρόνο αποθήκευσης του baseline του έργου.

```csharp
var project = new Project();
var baselineSave = project.GetBaselineSaveTime(BaselineType.Baseline);
Console.WriteLine("Baseline save time before: " + baselineSave);

// ορίστε χρόνο αποθήκευσης baseline
project.SetBaselineSaveTime(BaselineType.Baseline, DateTime.Today);

var baselineSaveNew = project.GetBaselineSaveTime(BaselineType.Baseline);
Console.WriteLine("Baseline save time after: " + baselineSaveNew);
```

### Δείτε επίσης

* enum [BaselineType](../../baselinetype/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


