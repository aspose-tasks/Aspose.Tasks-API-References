---
title: "Απαρίθμηση Shape"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Aspose.Tasks.Visualization.Shape enum. Σχήμα ενός δείκτη στην αρχή ή στο τέλος του στυλ μπάρας που θα αποδοθεί κατά την αποθήκευση δεδομένων προβολής σε κάποιο από το SaveFileFormat"
type: docs
weight: 3360
url: /el/net/aspose.tasks.visualization/shape/
---
## Shape enumeration

Σχήμα ενός δείκτη στην αρχή ή στο τέλος του στυλ μπάρας που θα αποδοθεί κατά την αποθήκευση δεδομένων προβολής σε κάποιο από το [`SaveFileFormat`](../../aspose.tasks.saving/savefileformat/).

```csharp
public enum Shape
```

### Τιμές

| Όνομα | Τιμή | Περιγραφή |
| --- | --- | --- |
| None | `0` | Δείχνει σχήμα None. |
| VerticalLine | `1` | Δείχνει σχήμα κατακόρυφης γραμμής. |
| Pentagon | `2` | Δείχνει σχήμα πενταγώνου. |
| Triangle | `3` | Δείχνει σχήμα τριγώνου. |
| LeftBracket | `4` | Δείχνει σχήμα αριστερής αγκύλης. |
| RightBracket | `5` | Δείχνει σχήμα δεξιάς αγκύλης. |
| ArrowDown | `6` | Δείχνει σχήμα ArrowDown. |
| LeftFade | `7` | Δείχνει σχήμα αριστερού fade. |
| RightFade | `8` | Δείχνει σχήμα δεξιού fade. |
| Diamond | `9` | Δείχνει σχήμα διαμαντικού. |
| Circle | `10` | Δείχνει σχήμα κύκλου. |

## Παραδείγματα

Δείχνει πώς να χρησιμοποιήσετε προσαρμοσμένα στυλ μπάρας.

```csharp
var project = new Project(DataDir + "Project2.mpp");
SaveOptions options = new PdfSaveOptions
{
    BarStyles = new List<BarStyle>()
};

// προσθέστε ένα στυλ μπάρας για εργασίες ορόσημου
var style = new BarStyle();
// ορίστε <see cref=\"T:Aspose.Tasks.Visualization.BarItemType\" /> του στυλ μπάρας
style.ItemType = BarItemType.Milestone;
// ορίστε <see cref=\"T:System.Drawing.Color\" /> του στυλ μπάρας.
style.BarColor = Color.Green;
// ορίστε <see cref=\"P:Aspose.Tasks.Visualization.BarStyle.BarShape\" /> του στυλ μπάρας
style.BarShape = BarShape.HalfHeight;
// ορίστε <see cref="T:Aspose.Tasks.Visualization.Shape" /> στην αρχή της μπάρας
style.StartShape = Shape.LeftBracket;
// ορίστε <see cref="T:System.Drawing.Color" /> του σχήματος στην αρχή της μπάρας
style.StartShapeColor = Color.Aqua;
// ορίστε <see cref="T:Aspose.Tasks.Visualization.Shape" /> στο τέλος της μπάρας
style.EndShape = Shape.RightBracket;
// ορίστε <see cref="T:System.Drawing.Color" /> του σχήματος στο τέλος της μπάρας
style.EndShapeColor = Color.Aquamarine;
// Ορίστε το κείμενο για απόδοση στα δεξιά της μπάρας.
style.TextStyle = new TextStyle();
style.TextStyle.BackgroundColor = Color.Black;

// Υπάρχει μια δυνατότητα που επιτρέπει τη μετατροπή κειμένου της μπάρας.
// Ας ορίσουμε τον μετατροπέα για να πάρουμε το κείμενο της μπάρας για απόδοση.
style.LeftBarTextConverter = task =>
{
    if (!task.Get(Tsk.Name).StartsWith("T"))
    {
        task.Set(Tsk.Name, "T" + task.Get(Tsk.Name));
    }

    return task.Get(Tsk.Name);
};

options.BarStyles.Add(style);

// Αποθηκεύστε το έργο
project.Save(OutDir + "WorkWithBarStyle_out.mpp", options);
```

### Δείτε επίσης

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


