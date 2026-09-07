---
title: "CsvOptions.DataCategory"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Ιδιότητα CsvOptions. Λαμβάνει ή ορίζει μια κατηγορία δεδομένων προς αποθήκευση."
type: docs
weight: 20
url: /el/net/aspose.tasks.saving/csvoptions/datacategory/
---
## CsvOptions.DataCategory property

Λαμβάνει ή ορίζει μια κατηγορία δεδομένων προς αποθήκευση.

```csharp
public DataCategory DataCategory { get; set; }
```

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

* enum [DataCategory](../../datacategory/)
* class [CsvOptions](../)
* namespace [Aspose.Tasks.Saving](../../csvoptions/)
* assembly [Aspose.Tasks](../../../)


