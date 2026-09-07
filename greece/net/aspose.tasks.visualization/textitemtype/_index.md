---
title: "Αρίθμηση TextItemType"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Αρίθμηση Aspose.Tasks.Visualization.TextItemType. Τύπος στοιχείου για την αλλαγή ενός στυλ κειμένου"
type: docs
weight: 3410
url: /el/net/aspose.tasks.visualization/textitemtype/
---
## TextItemType enumeration

Τύπος στοιχείου για αλλαγή στυλ κειμένου.

```csharp
public enum TextItemType
```

### Τιμές

| Όνομα | Τιμή | Περιγραφή |
| --- | --- | --- |
| RowColumnTitles | `0` | Τίτλοι γραμμής και στήλης. |
| CriticalTasks | `1` | Κρίσιμες εργασίες. |
| NoncriticalTasks | `2` | Μη κρίσιμες εργασίες. |
| MilestoneTasks | `3` | Εργασίες ορόσημου. |
| InactiveTasks | `4` | Ανενεργές εργασίες. |
| SummaryTasks | `5` | Συνοπτικές εργασίες. |
| AssignmentRow | `6` | Γραμμή ανάθεσης. |
| TopTimescaleTier | `7` | Ανώτερο επίπεδο χρονολογίας. |
| BottomTimescaleTier | `8` | Κατώτερο επίπεδο χρονολογίας. |
| MiddleTimescaleTier | `9` | Μεσαίο επίπεδο χρονολογίας. |
| Resources | `10` | Φύλλο πόρων. |
| OverallocatedResources | `11` | Υπερκατανεμημένοι πόροι. |
| TaskFilterHighlight | `12` | Στοιχείο κειμένου επισήμανσης φίλτρου εργασίας. |
| BarTextBottom | `13` | Στοιχείο κειμένου κάτω μπάρας. |
| BarTextInside | `14` | Στοιχείο κειμένου μέσα στη μπάρα. |
| BarTextLeft | `15` | Στοιχείο κειμένου αριστερά της μπάρας. |
| BarTextRight | `16` | Στοιχείο κειμένου δεξιά της μπάρας. |
| BarTextTop | `17` | Στοιχείο κειμένου πάνω μπάρας. |
| MarkedTasks | `18` | Στοιχείο κειμένου σημειωμένης εργασίας. |
| ProjectSummary | `19` | Στοιχείο κειμένου εργασίας σύνοψης έργου. |
| ExternalTasks | `20` | Στοιχείο κειμένου εξωτερικών εργασιών. |
| Allocated | `21` | Στοιχείο κειμένου κατανεμημένο. |
| ChangedCells | `22` | Αλλαγμένα κελιά. |

## Παραδείγματα

Δείχνει πώς να εργάζεστε με τύπους στοιχείων κειμένου.

```csharp
var project = new Project(DataDir + "CreateProject2.mpp");
SaveOptions options = new PdfSaveOptions
{
    PresentationFormat = PresentationFormat.ResourceSheet
};

var style = new TextStyle(FontStyles.Italic | FontStyles.Bold)
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

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


