---
title: "CsvOptions.Encoding"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Ιδιότητα CsvOptions. Λαμβάνει ή ορίζει μια κωδικοποίηση για αποθήκευση του CSV."
type: docs
weight: 30
url: /el/net/aspose.tasks.saving/csvoptions/encoding/
---
## CsvOptions.Encoding property

Λαμβάνει ή ορίζει μια κωδικοποίηση με την οποία θα αποθηκευτεί το CSV.

```csharp
public Encoding Encoding { get; set; }
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

* class [CsvOptions](../)
* namespace [Aspose.Tasks.Saving](../../csvoptions/)
* assembly [Aspose.Tasks](../../../)


