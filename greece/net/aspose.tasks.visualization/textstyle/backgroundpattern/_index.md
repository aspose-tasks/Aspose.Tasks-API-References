---
title: "TextStyle.BackgroundPattern"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Ιδιότητα TextStyle. Λαμβάνει ή ορίζει το μοτίβο φόντου του στυλ κειμένου. BackgroundPattern"
type: docs
weight: 30
url: /el/net/aspose.tasks.visualization/textstyle/backgroundpattern/
---
## TextStyle.BackgroundPattern property

Αποκτά ή ορίζει το μοτίβο φόντου του στυλ κειμένου. `BackgroundPattern`.

```csharp
public BackgroundPattern BackgroundPattern { get; set; }
```

## Παραδείγματα

Δείχνει πώς να προσαρμόσετε τα στυλ κειμένου που χρησιμοποιούνται για τη μορφοποίηση διαφορετικών στοιχείων κειμένου σε ένα έργο.

```csharp
var project = new Project(DataDir + "CreateProject2.mpp");
SaveOptions options = new PdfSaveOptions
{
    PresentationFormat = PresentationFormat.ResourceSheet
};

var style = new TextStyle();
style.Color = Color.OrangeRed;
style.Font = new FontDescriptor(FontFamily.GenericMonospace.Name, 10F, FontStyles.Bold | FontStyles.Italic);
style.ItemType = TextItemType.OverallocatedResources;
style.BackgroundColor = Color.Aqua;
style.BackgroundPattern = BackgroundPattern.DarkDither;

options.TextStyles = new List<TextStyle>
{
    style
};
project.Save(OutDir + "CustomizeTextStyle_out.pdf", options);
```

### Δείτε επίσης

* enum [BackgroundPattern](../../../aspose.tasks/backgroundpattern/)
* class [TextStyle](../)
* namespace [Aspose.Tasks.Visualization](../../textstyle/)
* assembly [Aspose.Tasks](../../../)


