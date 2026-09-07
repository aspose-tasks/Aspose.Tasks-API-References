---
title: "TextStyle.TextStyle"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Κατασκευαστής TextStyle. Αρχικοποιεί ένα νέο αντικείμενο της κλάσης TextStyle με προεπιλεγμένες ρυθμίσεις"
type: docs
weight: 10
url: /el/net/aspose.tasks.visualization/textstyle/textstyle/
---
## TextStyle() {#constructor}

Αρχικοποιεί ένα νέο αντικείμενο της κλάσης [`TextStyle`](../) με προεπιλεγμένες ρυθμίσεις.

```csharp
public TextStyle()
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

* class [TextStyle](../)
* namespace [Aspose.Tasks.Visualization](../../textstyle/)
* assembly [Aspose.Tasks](../../../)

---

## TextStyle(float, FontStyles) {#constructor_3}

Αρχικοποιεί ένα νέο αντικείμενο της κλάσης [`TextStyle`](../) με την προεπιλεγμένη γραμματοσειρά και το καθορισμένο μέγεθος και στυλ γραμματοσειράς.

```csharp
public TextStyle(float fontSize, FontStyles fontStyle)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| fontSize | Single | Μέγεθος γραμματοσειράς του TextStyle. |
| fontStyle | FontStyles | Στυλ γραμματοσειράς του TextStyle. |

### Δείτε επίσης

* enum [FontStyles](../../fontstyles/)
* class [TextStyle](../)
* namespace [Aspose.Tasks.Visualization](../../textstyle/)
* assembly [Aspose.Tasks](../../../)

---

## TextStyle(FontStyles) {#constructor_2}

Αρχικοποιεί ένα νέο αντικείμενο της κλάσης [`TextStyle`](../) με την προεπιλεγμένη γραμματοσειρά και το καθορισμένο στυλ γραμματοσειράς.

```csharp
public TextStyle(FontStyles fontStyle)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| fontStyle | FontStyles | Στυλ γραμματοσειράς που εφαρμόζεται στην προεπιλεγμένη γραμματοσειρά. |

### Δείτε επίσης

* enum [FontStyles](../../fontstyles/)
* class [TextStyle](../)
* namespace [Aspose.Tasks.Visualization](../../textstyle/)
* assembly [Aspose.Tasks](../../../)

---

## TextStyle(FontDescriptor) {#constructor_1}

Αρχικοποιεί ένα νέο αντικείμενο της κλάσης [`TextStyle`](../) με τις καθορισμένες ρυθμίσεις γραμματοσειράς.

```csharp
public TextStyle(FontDescriptor font)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| font | FontDescriptor | Γραμματοσειρά του TextStyle. |

### Δείτε επίσης

* class [FontDescriptor](../../fontdescriptor/)
* class [TextStyle](../)
* namespace [Aspose.Tasks.Visualization](../../textstyle/)
* assembly [Aspose.Tasks](../../../)


