---
title: "Project.SetBaselineSaveTime"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Project method. Ορίζει το χρόνο αποθήκευσης του baseline"
type: docs
weight: 1260
url: /el/net/aspose.tasks/project/setbaselinesavetime/
---
## Project.SetBaselineSaveTime method

Ορίζει την ώρα αποθήκευσης του baseline.

```csharp
public void SetBaselineSaveTime(BaselineType baselineNumber, DateTime value)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| baselineNumber | BaselineType | Ο αριθμός του baseline [`BaselineType`](../../baselinetype/). |
| value | DateTime | Η τελευταία ημερομηνία και ώρα αποθήκευσης του baseline. |

## Παρατηρήσεις

Ορίστε την τιμή σε DateTime.MinValue εάν το baseline δεν έχει αποθηκευτεί.

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


