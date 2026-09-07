---
title: "Κλάση TextStyle"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Aspose.Tasks.Visualization.TextStyle class. Αλλάξτε το οπτικό στυλ του κειμένου για ένα στοιχείο στην προβολή του έργου"
type: docs
weight: 3420
url: /el/net/aspose.tasks.visualization/textstyle/
---
## TextStyle class

Αλλάξτε το οπτικό στυλ του κειμένου για ένα στοιχείο στην προβολή του έργου.

```csharp
public class TextStyle
```

## Κατασκευαστές

| Όνομα | Περιγραφή |
| --- | --- |
| [TextStyle](textstyle/#constructor)() | Αρχικοποιεί ένα νέο αντικείμενο της κλάσης `TextStyle` με προεπιλεγμένες ρυθμίσεις. |
| [TextStyle](textstyle/#constructor_1)(FontDescriptor) | Αρχικοποιεί ένα νέο αντικείμενο της κλάσης `TextStyle` με τις καθορισμένες ρυθμίσεις γραμματοσειράς. |
| [TextStyle](textstyle/#constructor_2)(FontStyles) | Αρχικοποιεί ένα νέο αντικείμενο της κλάσης `TextStyle` με την προεπιλεγμένη γραμματοσειρά και το καθορισμένο στυλ γραμματοσειράς. |
| [TextStyle](textstyle/#constructor_3)(float, FontStyles) | Αρχικοποιεί ένα νέο αντικείμενο της κλάσης `TextStyle` με την προεπιλεγμένη γραμματοσειρά και το καθορισμένο μέγεθος και στυλ γραμματοσειράς. |

## Ιδιότητες

| Όνομα | Περιγραφή |
| --- | --- |
| [BackgroundColor](../../aspose.tasks.visualization/textstyle/backgroundcolor/) { get; set; } | Λαμβάνει ή ορίζει το χρώμα φόντου του στυλ κειμένου. [`Color`](./color/). |
| [BackgroundPattern](../../aspose.tasks.visualization/textstyle/backgroundpattern/) { get; set; } | Λαμβάνει ή ορίζει το μοτίβο φόντου του στυλ κειμένου. [`BackgroundPattern`](./backgroundpattern/). |
| [Color](../../aspose.tasks.visualization/textstyle/color/) { get; set; } | Λαμβάνει ή ορίζει το χρώμα του κειμένου. |
| [Font](../../aspose.tasks.visualization/textstyle/font/) { get; set; } | Λαμβάνει ή ορίζει τη γραμματοσειρά του στυλ κειμένου. |
| virtual [ItemType](../../aspose.tasks.visualization/textstyle/itemtype/) { get; set; } | Λαμβάνει ή ορίζει το [`TextItemType`](../textitemtype/) του στυλ κειμένου. |

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

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


