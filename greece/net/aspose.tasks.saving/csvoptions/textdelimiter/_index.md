---
title: "CsvOptions.TextDelimiter"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Ιδιότητα CsvOptions. Λαμβάνει ή ορίζει έναν οριοθέτη κειμένου"
type: docs
weight: 50
url: /el/net/aspose.tasks.saving/csvoptions/textdelimiter/
---
## CsvOptions.TextDelimiter property

Λαμβάνει ή ορίζει ένα διαχωριστικό κειμένου.

```csharp
public CsvTextDelimiter TextDelimiter { get; set; }
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

* enum [CsvTextDelimiter](../../csvtextdelimiter/)
* class [CsvOptions](../)
* namespace [Aspose.Tasks.Saving](../../csvoptions/)
* assembly [Aspose.Tasks](../../../)


