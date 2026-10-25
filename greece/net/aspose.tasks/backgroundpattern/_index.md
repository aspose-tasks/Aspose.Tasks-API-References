---
title: "Απαρίθμηση BackgroundPattern"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Απαρίθμηση Aspose.Tasks.BackgroundPattern. Καθορίζει το μοτίβο φόντου"
type: docs
weight: 100
url: /el/net/aspose.tasks/backgroundpattern/
---
## BackgroundPattern enumeration

Καθορίζει το μοτίβο φόντου.

```csharp
public enum BackgroundPattern
```

### Τιμές

| Όνομα | Τιμή | Περιγραφή |
| --- | --- | --- |
| DarkDiagonalLeft | `7` | Δείχνει το σκοτεινό διαγώνιο αριστερό μοτίβο φόντου. |
| DarkDiagonalRight | `8` | Δείχνει το σκοτεινό διαγώνιο δεξιό μοτίβο φόντου. |
| DarkDither | `13` | Δείχνει το σκοτεινό μοτίβο θόλωσης φόντου. |
| DarkFill | `4` | Δείχνει το σκοτεινό μοτίβο γεμίσματος φόντου. |
| DiagonalLeft | `5` | Δείχνει το διαγώνιο αριστερό μοτίβο φόντου. |
| DiagonalRight | `6` | Δείχνει το διαγώνιο δεξιό μοτίβο φόντου. |
| Hollow | `0` | Δείχνει το κενό μοτίβο φόντου. |
| LightDither | `11` | Δείχνει το ελαφρύ μοτίβο δισδιάστατου φόντου. |
| LightFill | `2` | Δείχνει το ελαφρύ μοτίβο γεμίσματος φόντου. |
| MediumDither | `12` | Δείχνει το μεσαίο μοτίβο δισδιάστατου φόντου. |
| MediumFill | `3` | Δείχνει το μεσαίο μοτίβο γεμίσματος φόντου. |
| MediumVerticalStripe | `10` | Δείχνει το μεσαίο κάθετο λωρίδα μοτίβου φόντου. |
| SolidFill | `1` | Δείχνει το συμπαγές μοτίβο γεμίσματος φόντου. |
| ThinVerticalStripe | `9` | Δείχνει το λεπτό κάθετο λωρίδα μοτίβου φόντου. |

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


