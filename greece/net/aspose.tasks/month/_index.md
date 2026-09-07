---
title: "Απαρίθμηση Month"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Aspose.Tasks.Month απαρίθμηση. Καθορίζει το μήνα"
type: docs
weight: 1040
url: /el/net/aspose.tasks/month/
---
## Month enumeration

Καθορίζει το μήνα.

```csharp
public enum Month
```

### Τιμές

| Όνομα | Τιμή | Περιγραφή |
| --- | --- | --- |
| Undefined | `-1` | Δείχνει ότι η τιμή δεν ορίστηκε στο αρχικό αρχείο έργου. |
| January | `0` | Υποδεικνύει τον μήνα Ιανουάριο. |
| February | `1` | Υποδεικνύει τον μήνα Φεβρουάριο. |
| March | `2` | Υποδεικνύει τον μήνα Μάρτιο. |
| April | `3` | Υποδεικνύει τον μήνα Απρίλιο. |
| May | `4` | Υποδεικνύει τον μήνα Μάι. |
| June | `5` | Υποδεικνύει τον μήνα Ιούνιο. |
| July | `6` | Υποδεικνύει τον μήνα Ιούλιο. |
| August | `7` | Υποδεικνύει τον μήνα Αύγουστο. |
| September | `8` | Υποδεικνύει τον μήνα Σεπτέμβριο. |
| October | `9` | Υποδεικνύει τον μήνα Οκτώβριο. |
| November | `10` | Υποδεικνύει τον μήνα Νοέμβριο. |
| December | `11` | Υποδεικνύει τον μήνα Δεκέμβριο. |

## Παρατηρήσεις

Κατά την εξαγωγή σε XML, οι μη ορισμένες τιμές θα αφαιρεθούν από το τελικό XML.

## Παραδείγματα

Εμφανίζει πώς να εργαστείτε με επαναλήψεις ημερών του έτους ενώ δημιουργείτε νέες επαναλαμβανόμενες εργασίες.

```csharp
var project = new Project(DataDir + "Project1.mpp");
var parameters = new RecurringTaskParameters
                     {
                         TaskName = "t1",
                         Duration = project.GetDuration(1, TimeUnitType.Day),
                         RecurrencePattern = new YearlyRecurrencePattern
                                                 {
                                                     Repetition = new ByYearDayRepetition { DayPosition = 1, Month = Month.July },
                                                     RecurrenceRange = new EndByRecurrenceRange
                                                                           {
                                                                               Start = new DateTime(2018, 7, 1, 8, 0, 0),
                                                                               Finish = new DateTime(2019, 7, 1, 17, 0, 0)
                                                                           }
                                                 }
                     };
project.RootTask.Children.Add(parameters);

project.Save(OutDir + "CanAddRecurringTask_Years_YearDay_EndByRecurrenceRange_Test.mpp", SaveFileFormat.Mpp);
```

### Δείτε επίσης

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


