---
title: "CsvOptions.CsvOptions"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Κατασκευαστής CsvOptions. Αρχικοποιεί ένα νέο αντικείμενο της κλάσης CsvOptions που μπορεί να χρησιμοποιηθεί για αποθήκευση έργου σε μορφή CSV."
type: docs
weight: 10
url: /el/net/aspose.tasks.saving/csvoptions/csvoptions/
---
## CsvOptions constructor

Αρχικοποιεί ένα νέο αντικείμενο της κλάσης [`CsvOptions`](../) που μπορεί να χρησιμοποιηθεί για αποθήκευση έργου σε μορφή CSV.

```csharp
public CsvOptions()
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


