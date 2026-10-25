---
title: "Enum TaskStartDateType"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Aspose.Tasks.TaskStartDateType enum. Καθορίζει τον τύπο της ημερομηνίας έναρξης μιας εργασίας"
type: docs
weight: 2450
url: /el/net/aspose.tasks/taskstartdatetype/
---
## TaskStartDateType enumeration

Καθορίζει τον τύπο της ημερομηνίας έναρξης μιας εργασίας.

```csharp
public enum TaskStartDateType
```

### Τιμές

| Όνομα | Τιμή | Περιγραφή |
| --- | --- | --- |
| Undefined | `-1` | Η τιμή του πεδίου δεν ορίστηκε στο αρχικό αρχείο έργου. |
| ProjectStartDate | `0` | Ημερομηνία έναρξης έργου |
| CurrentDate | `1` | Τρέχουσα ημερομηνία |

## Παρατηρήσεις

Κατά την εξαγωγή σε XML, οι μη ορισμένες τιμές θα αφαιρεθούν από το τελικό XML.

## Παραδείγματα

Δείχνει πώς να ορίσετε την προεπιλεγμένη ημερομηνία έναρξης της εργασίας ως 'CurrentDate'.

```csharp
var project = new Project();
project.Set(Prj.NewTaskStartDate, TaskStartDateType.CurrentDate);
project.Save(OutDir + "SetAttributesForNewTasks_out.xml", SaveFileFormat.Xml);
```

### Δείτε επίσης

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


