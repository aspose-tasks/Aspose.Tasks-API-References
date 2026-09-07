---
title: "ImageSaveOptions.ReduceFooterGap"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Ιδιότητα ImageSaveOptions. Λαμβάνει ή ορίζει μια τιμή που υποδεικνύει εάν πρέπει να μειωθεί το κενό μεταξύ της τελευταίας εργασίας και του υποσέλιδου."
type: docs
weight: 80
url: /el/net/aspose.tasks.saving/imagesaveoptions/reducefootergap/
---
## ImageSaveOptions.ReduceFooterGap property

Αποκτά ή ορίζει μια τιμή που υποδεικνύει εάν το κενό μεταξύ της τελευταίας εργασίας και του υποσέλιδου πρέπει να μειωθεί.

```csharp
public bool ReduceFooterGap { get; set; }
```

## Παραδείγματα

Δείχνει πώς να ορίσετε μια τιμή που υποδεικνύει εάν πρέπει να μειωθεί το κενό μεταξύ της τελευταίας εργασίας και του υποσέλιδου.

```csharp
var project = new Project(DataDir + "CreateProject2.mpp");

// Χρησιμοποιήστε την ιδιότητα ReduceFooterGap για να μειώσετε το κενό μεταξύ της λίστας εργασιών και του υποσέλιδου.
var imageSaveOptions = new ImageSaveOptions(SaveFileFormat.Png)
                           {
                               ReduceFooterGap = true, /* set to true */ 
                               RenderToSinglePage = false,
                               PageSize = PageSize.A0,
                               Timescale = Timescale.Days
                           };
project.Save(OutDir + "ReducingGapBetweenTasksListAndFooter_out.png", imageSaveOptions);
```

### Δείτε επίσης

* class [ImageSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../imagesaveoptions/)
* assembly [Aspose.Tasks](../../../)


