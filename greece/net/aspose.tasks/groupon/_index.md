---
title: "Enum GroupOn"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Aspose.Tasks.GroupOn enum. Καθορίζει τον τύπο ομαδοποίησης"
type: docs
weight: 810
url: /el/net/aspose.tasks/groupon/
---
## GroupOn enumeration

Καθορίζει τον τύπο ομαδοποίησης.

```csharp
public enum GroupOn
```

### Τιμές

| Όνομα | Τιμή | Περιγραφή |
| --- | --- | --- |
| DateDay | `13` | Ομαδοποίηση κατά ημερομηνία ανά ημέρα. |
| DateEachValue | `10` | Ομαδοποίηση κατά ημερομηνία για κάθε τιμή. |
| DateHour | `12` | Ομαδοποίηση κατά ημερομηνία ανά ώρα. |
| DateMinute | `11` | Ομαδοποίηση κατά ημερομηνία ανά λεπτό. |
| DateMonth | `16` | Ομαδοποίηση κατά ημερομηνία ανά μήνα. |
| DateQtr | `17` | Ομαδοποίηση κατά ημερομηνία ανά τρίμηνο. |
| DateThirdOfMonth | `15` | Ομαδοποίηση κατά ημερομηνία ανά κάθε τρίτο του μήνα. |
| DateWeek | `14` | Ομαδοποίηση κατά ημερομηνία ανά εβδομάδα. |
| DateYear | `18` | Ομαδοποίηση κατά ημερομηνία ανά έτος. |
| DurationDays | `23` | Ομαδοποίηση κατά διάρκεια ανά ημέρες. |
| DurationEachValue | `20` | Ομαδοποίηση κατά διάρκεια για κάθε τιμή. |
| DurationHours | `22` | Ομαδοποίηση κατά διάρκεια ανά ώρες. |
| DurationMinutes | `21` | Ομαδοποίηση κατά διάρκεια ανά λεπτά. |
| DurationMonths | `25` | Ομαδοποίηση κατά διάρκεια ανά μήνες. |
| DurationWeeks | `24` | Ομαδοποίηση κατά διάρκεια ανά εβδομάδες. |
| EachValue | `0` | Ομαδοποίηση ανά κάθε τιμή. |
| Interval | `1` | Ομαδοποίηση ανά το διάστημα. |
| OutlineEachValue | `30` | Ομαδοποίηση ανά κάθε τιμή περιγράμματος. |
| OutlineLevel | `31` | Ομαδοποίηση ανά επίπεδο περιγράμματος. |
| Pct110 | `45` | Ομαδοποίηση ανά βήματα ολοκλήρωσης 10%. |
| Pct125 | `44` | Ομαδοποίηση ανά βήματα ολοκλήρωσης 25%. |
| Pct150 | `43` | Ομαδοποίηση ανά βήματα ολοκλήρωσης 50%. |
| Pct199 | `42` | Ομαδοποίηση ανά 99% ολοκλήρωση. |
| PctEachValue | `40` | Ομαδοποίηση κατά ποσοστό κάθε τιμής. |
| PctInterval | `41` | Ομαδοποίηση κατά ποσοστό διαστήματος. |
| TextEachValue | `50` | Ομαδοποίηση ανά κάθε κειμενική τιμή. |
| TextPrefix | `51` | Ομαδοποίηση κατά πρόθεμα κειμένου. |

## Παραδείγματα

Δείχνει πώς να διαβάσετε τις ιδιότητες ενός κριτηρίου ομάδας.

```csharp
var project = new Project(DataDir + "ReadGroupDefinitionData.mpp");

Console.WriteLine("Task Groups Count: " + project.TaskGroups.Count);
var group = project.TaskGroups.ToList()[1];
Console.WriteLine("Task Group Name: " + group.Name);
Console.WriteLine("Task Group Criteria count: " + group.GroupCriteria.Count);

Console.WriteLine("\n************* Retrieving Task Group's Criterion information *************");
var criterion = group.GroupCriteria.ToList()[0];
Console.WriteLine("Task Criterion Field: " + criterion.Field);
Console.WriteLine("Task Criterion GroupOn: " + criterion.GroupOn);
Console.WriteLine("Task Criterion Cell Color: " + criterion.CellColor);
Console.WriteLine("Task Criterion Font Color: " + criterion.FontColor);
Console.WriteLine("Task Criterion Group Interval: " + criterion.GroupInterval);
Console.WriteLine("Task Criterion Start At: " + criterion.StartAt);

// Διαβάστε το υπόβαθρο του προτύπου του κριτηρίου.
Console.WriteLine("Task Criterion Pattern: " + criterion.Pattern);

Console.WriteLine("\n*********** Retrieving Criterion's Font Information ***********");
Console.WriteLine("Font Name: " + criterion.Font.FontFamily);
Console.WriteLine("Font Size: " + criterion.Font.Size);
Console.WriteLine("Font Style: " + criterion.Font.Style);
Console.WriteLine("Ascending/Descending: " + criterion.Ascending);
```

### Δείτε επίσης

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


