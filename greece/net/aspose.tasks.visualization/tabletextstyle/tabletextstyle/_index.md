---
title: "TableTextStyle.TableTextStyle"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Κατασκευαστής TableTextStyle. Αρχικοποιεί ένα νέο στιγμιότυπο της κλάσης TableTextStyle."
type: docs
weight: 10
url: /el/net/aspose.tasks.visualization/tabletextstyle/tabletextstyle/
---
## TableTextStyle(int) {#constructor}

Αρχικοποιεί ένα νέο στιγμιότυπο της κλάσης [`TableTextStyle`](../).

```csharp
public TableTextStyle(int rowUid)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| rowUid | Int32 | Ένα καθορισμένο μοναδικό αναγνωριστικό γραμμής. |

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

* class [TableTextStyle](../)
* namespace [Aspose.Tasks.Visualization](../../tabletextstyle/)
* assembly [Aspose.Tasks](../../../)

---

## TableTextStyle(int, FontDescriptor) {#constructor_1}

Αρχικοποιεί ένα νέο στιγμιότυπο της κλάσης [`TableTextStyle`](../) με τη συγκεκριμένη γραμματοσειρά.

```csharp
public TableTextStyle(int rowUid, FontDescriptor font)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| rowUid | Int32 | Ένα καθορισμένο μοναδικό αναγνωριστικό γραμμής. |
| font | FontDescriptor | Μια γραμματοσειρά στην οποία βασίζεται ένα στυλ κειμένου. |

### Δείτε επίσης

* class [FontDescriptor](../../fontdescriptor/)
* class [TableTextStyle](../)
* namespace [Aspose.Tasks.Visualization](../../tabletextstyle/)
* assembly [Aspose.Tasks](../../../)

---

## TableTextStyle(int, float, FontStyles) {#constructor_3}

Αρχικοποιεί ένα νέο στιγμιότυπο της κλάσης [`TableTextStyle`](../) με το συγκεκριμένο μέγεθος γραμματοσειράς και στυλ γραμματοσειράς.

```csharp
public TableTextStyle(int rowUid, float fontSize, FontStyles fontStyle)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| rowUid | Int32 | Ένα καθορισμένο μοναδικό αναγνωριστικό γραμμής. |
| fontSize | Single | Μέγεθος μιας γραμματοσειράς στην οποία βασίζεται ένα στυλ κειμένου. |
| fontStyle | FontStyles | Στυλ μιας γραμματοσειράς στην οποία βασίζεται ένα στυλ κειμένου. |

### Δείτε επίσης

* enum [FontStyles](../../fontstyles/)
* class [TableTextStyle](../)
* namespace [Aspose.Tasks.Visualization](../../tabletextstyle/)
* assembly [Aspose.Tasks](../../../)

---

## TableTextStyle(int, FontStyles) {#constructor_2}

Αρχικοποιεί ένα νέο στιγμιότυπο της κλάσης [`TableTextStyle`](../) με τις προεπιλεγμένες ρυθμίσεις γραμματοσειράς και το καθορισμένο στυλ γραμματοσειράς.

```csharp
public TableTextStyle(int rowUid, FontStyles fontStyle)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| rowUid | Int32 | Ένα καθορισμένο μοναδικό αναγνωριστικό γραμμής. |
| fontStyle | FontStyles | Στυλ μιας γραμματοσειράς στην οποία βασίζεται ένα στυλ κειμένου. |

### Δείτε επίσης

* enum [FontStyles](../../fontstyles/)
* class [TableTextStyle](../)
* namespace [Aspose.Tasks.Visualization](../../tabletextstyle/)
* assembly [Aspose.Tasks](../../../)


