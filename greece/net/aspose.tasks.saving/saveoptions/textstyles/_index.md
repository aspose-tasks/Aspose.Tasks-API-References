---
title: "SaveOptions.TextStyles"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Ιδιότητα SaveOptions. Λαμβάνει ή ορίζει τη λίστα των στυλ κειμένου που εφαρμόζονται κατά την απόδοση μιας προβολής έργου."
type: docs
weight: 190
url: /el/net/aspose.tasks.saving/saveoptions/textstyles/
---
## SaveOptions.TextStyles property

Λαμβάνει ή ορίζει τη λίστα των στυλ κειμένου που εφαρμόζονται κατά την απόδοση μιας προβολής έργου.

```csharp
public List<TextStyle> TextStyles { get; set; }
```

## Παρατηρήσεις

Αυτά τα στυλ αντικαθιστούν τα στυλ που ορίζονται στο GanttCharView.TextStyles.

## Παραδείγματα

Δείχνει πώς να χρησιμοποιήσετε τα στυλ κειμένου των επιλογών αποθήκευσης που χρησιμοποιούνται για τη μορφοποίηση διαφορετικών **text items** σε ένα έργο.

```csharp
var project = new Project(DataDir + "CreateProject2.mpp");
SaveOptions options = new PdfSaveOptions
{
    PresentationFormat = PresentationFormat.ResourceSheet
};

var style = new TextStyle(FontStyles.Bold | FontStyles.Italic)
{
    Color = Color.OrangeRed
};

style.ItemType = TextItemType.OverallocatedResources;

options.TextStyles = new List<TextStyle>
{
    style
};

project.Save(OutDir + "CustomizeTextStyle_out.pdf", options);
```

### Δείτε επίσης

* class [TextStyle](../../../aspose.tasks.visualization/textstyle/)
* class [SaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../saveoptions/)
* assembly [Aspose.Tasks](../../../)


