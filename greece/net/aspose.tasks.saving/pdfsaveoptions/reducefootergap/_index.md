---
title: "PdfSaveOptions.ReduceFooterGap"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Ιδιότητα PdfSaveOptions. Λαμβάνει ή ορίζει μια τιμή που υποδεικνύει εάν το κενό μεταξύ της τελευταίας εργασίας και του υποσέλιδου πρέπει να μειωθεί."
type: docs
weight: 80
url: /el/net/aspose.tasks.saving/pdfsaveoptions/reducefootergap/
---
## PdfSaveOptions.ReduceFooterGap property

Αποκτά ή ορίζει μια τιμή που υποδεικνύει εάν το κενό μεταξύ της τελευταίας εργασίας και του υποσέλιδου πρέπει να μειωθεί.

```csharp
public bool ReduceFooterGap { get; set; }
```

## Παραδείγματα

Δείχνει πώς να ορίσετε μια τιμή που υποδεικνύει εάν το κενό μεταξύ της τελευταίας εργασίας και του υποσέλιδου πρέπει να μειωθεί στα αρχεία εξόδου PDF.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

var options = new PdfSaveOptions { ReduceFooterGap = true, PageSize = PageSize.A0, Timescale = Timescale.Days };

project.Save(OutDir + "ReducingGapBetweenTasksListAndFooter_out.pdf", options);
```

### Δείτε επίσης

* class [PdfSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../pdfsaveoptions/)
* assembly [Aspose.Tasks](../../../)


