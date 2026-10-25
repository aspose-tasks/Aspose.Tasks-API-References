---
title: "FontSettings.SetFontFolders"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Μέθοδος FontSettings. Ορίζει τους φακέλους όπου το Aspose.Tasks αναζητά γραμματοσειρές TrueType κατά την απόδοση της προβολής έργων"
type: docs
weight: 50
url: /el/net/aspose.tasks/fontsettings/setfontfolders/
---
## FontSettings.SetFontFolders method

Ορίζει τους φακέλους όπου το Aspose.Tasks αναζητά γραμματοσειρές TrueType κατά την απόδοση της προβολής του έργου.

```csharp
public void SetFontFolders(string[] fontFolders, bool recursive)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| fontFolders | String[] | Ένας πίνακας φακέλων που περιέχουν γραμματοσειρές TrueType. |
| recursive | Boolean | Εάν είναι true, οι καθορισμένοι φάκελοι θα σαρωθούν αναδρομικά. |

## Παραδείγματα

Δείχνει πώς να ορίσετε προσαρμοσμένο φάκελο γραμματοσειρών.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

var options = new PdfSaveOptions
{
    PresentationFormat = PresentationFormat.GanttChart,
};

// Τα αρχεία γραμματοσειρών TrueType για όλες τις γραμματοσειρές που χρησιμοποιούνται στο ανοιγμένο έργο πρέπει να βρίσκονται στον φάκελο MyFonts.
options.FontSettings.SetFontFolders(new string[] { "c:\\MyFonts"}, true);

project.Save(OutDir + "EstimatedMilestoneTasks_out4.pdf", options);
```

### Δείτε επίσης

* class [FontSettings](../)
* namespace [Aspose.Tasks](../../fontsettings/)
* assembly [Aspose.Tasks](../../../)


