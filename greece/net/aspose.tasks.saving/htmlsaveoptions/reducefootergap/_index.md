---
title: "HtmlSaveOptions.ReduceFooterGap"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Ιδιότητα HtmlSaveOptions. Λαμβάνει ή ορίζει μια τιμή που υποδεικνύει εάν πρέπει να μειωθεί το κενό μεταξύ της τελευταίας εργασίας και του υποσέλιδου."
type: docs
weight: 150
url: /el/net/aspose.tasks.saving/htmlsaveoptions/reducefootergap/
---
## HtmlSaveOptions.ReduceFooterGap property

Αποκτά ή ορίζει μια τιμή που υποδεικνύει εάν το κενό μεταξύ της τελευταίας εργασίας και του υποσέλιδου πρέπει να μειωθεί.

```csharp
public bool ReduceFooterGap { get; set; }
```

## Παραδείγματα

Δείχνει πώς να ορίσετε μια τιμή που υποδεικνύει εάν πρέπει να μειωθεί το κενό μεταξύ της τελευταίας εργασίας και του υποσέλιδου στα αρχεία εξόδου HTML.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

var options = new HtmlSaveOptions
                  {
                      ReduceFooterGap = true,
                      IncludeProjectNameInPageHeader = false,
                      IncludeProjectNameInTitle = false,
                      PageSize = PageSize.A0,
                      Timescale = Timescale.Days
                  };
project.Save(OutDir + "ReducingGapBetweenTasksListAndFooter_out.html", options);
```

### Δείτε επίσης

* class [HtmlSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../htmlsaveoptions/)
* assembly [Aspose.Tasks](../../../)


