---
title: "Κλάση TableTextStyle"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Aspose.Tasks.Visualization.TableTextStyle κλάση. Αντιπροσωπεύει ένα στυλ κειμένου σε έναν πίνακα προβολής"
type: docs
weight: 3370
url: /el/net/aspose.tasks.visualization/tabletextstyle/
---
## TableTextStyle class

Αναπαριστά ένα στυλ κειμένου σε πίνακα προβολής.

```csharp
public class TableTextStyle : TextStyle
```

## Κατασκευαστές

| Όνομα | Περιγραφή |
| --- | --- |
| [TableTextStyle](tabletextstyle/#constructor)(int) | Αρχικοποιεί ένα νέο αντικείμενο της κλάσης `TableTextStyle`. |
| [TableTextStyle](tabletextstyle/#constructor_1)(int, FontDescriptor) | Αρχικοποιεί ένα νέο αντικείμενο της κλάσης `TableTextStyle` με τη συγκεκριμένη γραμματοσειρά. |
| [TableTextStyle](tabletextstyle/#constructor_2)(int, FontStyles) | Αρχικοποιεί ένα νέο αντικείμενο της κλάσης `TableTextStyle` με τις προεπιλεγμένες ρυθμίσεις γραμματοσειράς και το συγκεκριμένο στυλ γραμματοσειράς. |
| [TableTextStyle](tabletextstyle/#constructor_3)(int, float, FontStyles) | Αρχικοποιεί ένα νέο αντικείμενο της κλάσης `TableTextStyle` με το συγκεκριμένο μέγεθος γραμματοσειράς και στυλ γραμματοσειράς. |

## Ιδιότητες

| Όνομα | Περιγραφή |
| --- | --- |
| [BackgroundColor](../../aspose.tasks.visualization/textstyle/backgroundcolor/) { get; set; } | Λαμβάνει ή ορίζει το χρώμα φόντου του στυλ κειμένου. [`Color`](../textstyle/color/). |
| [BackgroundPattern](../../aspose.tasks.visualization/textstyle/backgroundpattern/) { get; set; } | Λαμβάνει ή ορίζει το μοτίβο φόντου του στυλ κειμένου. [`BackgroundPattern`](../textstyle/backgroundpattern/). |
| [Color](../../aspose.tasks.visualization/textstyle/color/) { get; set; } | Λαμβάνει ή ορίζει το χρώμα του κειμένου. |
| [Field](../../aspose.tasks.visualization/tabletextstyle/field/) { get; set; } | Λαμβάνει ή ορίζει ένα πεδίο στο οποίο θα εφαρμοστεί το στυλ. [`Field`](./field/). |
| [Font](../../aspose.tasks.visualization/textstyle/font/) { get; set; } | Λαμβάνει ή ορίζει τη γραμματοσειρά του στυλ κειμένου. |
| override [ItemType](../../aspose.tasks.visualization/tabletextstyle/itemtype/) { get; } | Επιστρέφει μια τιμή του enum [`TextItemType`](../textitemtype/). |
| [RowUid](../../aspose.tasks.visualization/tabletextstyle/rowuid/) { get; } | Λαμβάνει ένα μοναδικό αναγνωριστικό γραμμής. Επιστρέφει -1 εάν το στυλ θα εφαρμοστεί σε όλες τις γραμμές μιας προβολής. |

## Παραδείγματα

Δείχνει πώς να προσαρμόσετε τα στυλ κειμένου πίνακα που χρησιμοποιούνται για τη μορφοποίηση διαφορετικών στοιχείων κειμένου σε ένα έργο.

```csharp
var project = new Project(DataDir + "Project2.mpp");
project.Set(Prj.NewTasksAreManual, false);

var view = (GanttChartView)project.Views.ToList()[0];

// ορίστε το στυλ κειμένου του πρώτου ονόματος εργασίας
var style1 = new TableTextStyle(1);
// ορίστε ένα πεδίο στο οποίο θα εφαρμοστεί το στυλ.
style1.Field = Field.TaskName;
// ορίστε <see cref="P:Aspose.Tasks.Visualization.TextStyle.Font" /> του στυλ κειμένου.
style1.Font = new FontDescriptor("Impact", 12F, FontStyles.Bold | FontStyles.Italic);
// ορίστε το μέγεθος σε σημεία της γραμματοσειράς του στυλ κειμένου.

// ορίστε το στυλ κειμένου της διάρκειας της δεύτερης εργασίας
var style2 = new TableTextStyle(2);
style2.Field = Field.TaskDurationText;
style2.Font = new FontDescriptor("Impact", 16F, FontStyles.Underline);

view.TableTextStyles.Add(style1);
view.TableTextStyles.Add(style2);

SimpleSaveOptions options = new MPPSaveOptions
{
    // ορίστε μια σημαία που υποδεικνύει ότι τα δεδομένα προβολής πρέπει να γραφούν
    WriteViewData = true
};
project.Save(OutDir + "WorkWithTableTextStyle_out.mpp", options);
```

### Δείτε επίσης

* class [TextStyle](../textstyle/)
* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


