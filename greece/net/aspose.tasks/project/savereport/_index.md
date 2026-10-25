---
title: "Project.SaveReport"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Μέθοδος Project. Αποθηκεύει την αναφορά επισκόπησης του έργου στο ρεύμα."
type: docs
weight: 1220
url: /el/net/aspose.tasks/project/savereport/
---
## SaveReport(Stream) {#savereport}

Αποθηκεύει την αναφορά επισκόπησης του έργου στη ροή.

```csharp
public void SaveReport(Stream stream)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| ροή | Ροή | Το ρεύμα στο οποίο θα αποθηκευτεί η αναφορά του έργου. |

## Παραδείγματα

Δείχνει πώς να αποθηκεύσετε την αναφορά επισκόπησης του έργου σε αρχείο PDF.

```csharp
var project = new Project(DataDir + "Cyclic structure.mpp");

// Αποθηκεύστε την αναφορά επισκόπησης σε αρχείο PDF στο καθορισμένο ρεύμα.
using (var stream = new FileStream(OutDir + "SaveProjectOverviewReport_out.pdf", FileMode.Create))
{
    project.SaveReport(stream);
}
```

### Δείτε επίσης

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## SaveReport(string) {#savereport_2}

Αποθηκεύει την αναφορά επισκόπησης του έργου σε αρχείο PDF.

```csharp
public void SaveReport(string fileName)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| fileName | String | Το όνομα αρχείου. |

## Παραδείγματα

Δείχνει πώς να αποθηκεύσετε την αναφορά επισκόπησης του έργου σε αρχείο PDF σε ένα ρεύμα.

```csharp
var project = new Project(DataDir + "Cyclic structure.mpp");

// Μπορείτε να αποθηκεύσετε την αναφορά επισκόπησης σε αρχείο PDF στην καθορισμένη διαδρομή.
project.SaveReport(OutDir + "SaveProjectOverviewReport_out.pdf");
```

### Δείτε επίσης

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## SaveReport(Stream, ReportType) {#savereport_1}

Αποθηκεύει την αναφορά του έργου του καθορισμένου τύπου στη καθορισμένη ροή.

```csharp
public void SaveReport(Stream stream, ReportType reportType)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| ροή | Ροή | το καθορισμένο ρεύμα για αποθήκευση της αναφοράς του έργου. |
| reportType | ReportType | ο καθορισμένος τύπος αναφοράς.[`ReportType`](../../../aspose.tasks.visualization/reporttype/) |

## Παραδείγματα

Δείχνει πώς να αποθηκεύσετε την αναφορά του έργου σε αρχείο PDF για συγκεκριμένο τύπο αναφοράς.

```csharp
var project = new Project(DataDir + "Cyclic structure.mpp");

// Αποθηκεύστε την αναφορά επισκόπησης σε αρχείο PDF στο καθορισμένο ρεύμα.
using (var stream = new FileStream(OutDir + "SaveProjectOverviewReport_out.pdf", FileMode.Create))
{
    project.SaveReport(stream, ReportType.Burndown);
}
```

### Δείτε επίσης

* enum [ReportType](../../../aspose.tasks.visualization/reporttype/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## SaveReport(string, ReportType) {#savereport_3}

Αποθηκεύει την αναφορά του έργου του καθορισμένου τύπου σε μορφή PDF στη καθορισμένη διαδρομή αρχείου.

```csharp
public void SaveReport(string fileName, ReportType reportType)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| fileName | String | το καθορισμένο όνομα αρχείου. |
| reportType | ReportType | ο καθορισμένος τύπος αναφοράς.[`ReportType`](../../../aspose.tasks.visualization/reporttype/) |

## Παραδείγματα

Δείχνει πώς να αποθηκεύσετε την αναφορά του έργου project σε μορφή PDF.

```csharp
var project = new Project(DataDir + "OzBuild 16 Orig.mpp");
project.SaveReport(OutDir + "CostOverview_out.pdf", ReportType.CostOverview);
```

### Δείτε επίσης

* enum [ReportType](../../../aspose.tasks.visualization/reporttype/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


