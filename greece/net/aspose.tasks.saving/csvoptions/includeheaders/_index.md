---
title: "CsvOptions.IncludeHeaders"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Ιδιότητα CsvOptions. Λαμβάνει ή ορίζει μια τιμή που υποδεικνύει εάν θα συμπεριληφθούν κεφαλίδες ή όχι· η προεπιλεγμένη τιμή είναι TRUE."
type: docs
weight: 40
url: /el/net/aspose.tasks.saving/csvoptions/includeheaders/
---
## CsvOptions.IncludeHeaders property

Λαμβάνει ή ορίζει μια τιμή που υποδεικνύει εάν θα συμπεριληφθούν κεφαλίδες ή όχι (η προεπιλεγμένη τιμή είναι TRUE).

```csharp
public bool IncludeHeaders { get; set; }
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


