---
title: "Enum DataCategory"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Η απαρίθμηση Aspose.Tasks.Saving.DataCategory. Η κατηγορία δεδομένων που χρησιμοποιείται κατά την αποθήκευση σε CSV"
type: docs
weight: 2000
url: /el/net/aspose.tasks.saving/datacategory/
---
## DataCategory enumeration

Η κατηγορία των δεδομένων που χρησιμοποιείται κατά την αποθήκευση σε CSV.

```csharp
public enum DataCategory
```

### Τιμές

| Όνομα | Τιμή | Περιγραφή |
| --- | --- | --- |
| Tasks | `0` | Πληροφορίες εργασιών. |
| Resources | `1` | Πληροφορίες πόρων. |
| Assignments | `2` | Πληροφορίες εκχωρήσεων. |

## Παραδείγματα

Δείχνει πώς να χρησιμοποιήσετε &lt;see cref=\"Aspose.Tasks.Saving.CsvOptions\" /&gt; για να αποθηκεύσετε ένα έργο ως αρχείο CSV.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");
var options = new CsvOptions
{
    DataCategory = DataCategory.Resources,
    TextDelimiter = CsvTextDelimiter.Semicolon,
    Encoding = Encoding.Unicode, IncludeHeaders = true
};

project.Save(OutDir + "WorkWithCsvOptions_out.csv", options);
```

### Δείτε επίσης

* namespace [Aspose.Tasks.Saving](../../aspose.tasks.saving/)
* assembly [Aspose.Tasks](../../)


