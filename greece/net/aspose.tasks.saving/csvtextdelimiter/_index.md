---
title: "Απαρίθμηση CsvTextDelimiter"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Απαρίθμηση Aspose.Tasks.Saving.CsvTextDelimiter. Διαχωριστικό κειμένου για μορφή CSV"
type: docs
weight: 1990
url: /el/net/aspose.tasks.saving/csvtextdelimiter/
---
## CsvTextDelimiter enumeration

Διαχωριστικό κειμένου για μορφή CSV.

```csharp
public enum CsvTextDelimiter
```

### Τιμές

| Όνομα | Τιμή | Περιγραφή |
| --- | --- | --- |
| Comma | `0` | Διαχωριστικό κόμμα. |
| Semicolon | `1` | Διαχωριστικό ερωτηματικού. |
| Space | `2` | Διαχωριστικό διαστήματος. |
| Tab | `3` | Διαχωριστικό στηλοθέτη. |

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


