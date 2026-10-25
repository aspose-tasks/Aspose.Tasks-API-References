---
title: "ImageSaveOptions.Pages"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Ιδιότητα ImageSaveOptions. Λαμβάνει ή ορίζει μια λίστα αριθμών σελίδων για αποθήκευση όταν αποθηκεύεται η διάταξη του έργου σε ξεχωριστά αρχεία. Όλες οι σελίδες θα αποθηκευτούν εάν αυτή η λίστα είναι κενή."
type: docs
weight: 50
url: /el/net/aspose.tasks.saving/imagesaveoptions/pages/
---
## ImageSaveOptions.Pages property

Λαμβάνει ή ορίζει μια λίστα αριθμών σελίδων που θα αποθηκευτούν όταν αποθηκεύεται η διάταξη του έργου σε ξεχωριστά αρχεία. Όλες οι σελίδες θα αποθηκευτούν εάν αυτή η λίδα είναι κενή.

```csharp
public List<int> Pages { get; set; }
```

## Παραδείγματα

Δείχνει πώς να αποθηκεύσετε τις επιλεγμένες σελίδες ως εικόνα.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

var options = new ImageSaveOptions(SaveFileFormat.Jpeg)
                  {
                      RenderToSinglePage = false,
                      StartDate = project.Get(Prj.StartDate),
                      EndDate = project.Get(Prj.FinishDate),
                      PageSize = PageSize.Letter
                  };
options.Pages.Add(2);

project.Save(OutDir + "SaveSelectedPagesImageSaveOptions_page2_out.jpeg", options);
```

### Δείτε επίσης

* class [ImageSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../imagesaveoptions/)
* assembly [Aspose.Tasks](../../../)


