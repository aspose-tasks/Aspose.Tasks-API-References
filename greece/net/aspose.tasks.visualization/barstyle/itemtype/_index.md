---
title: "BarStyle.ItemType"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Ιδιότητα BarStyle. Λαμβάνει ή ορίζει το BarItemType του στυλ μπάρας"
type: docs
weight: 120
url: /el/net/aspose.tasks.visualization/barstyle/itemtype/
---
## BarStyle.ItemType property

Λαμβάνει ή ορίζει το [`BarItemType`](../../baritemtype/) του στυλ μπάρας.

```csharp
public BarItemType ItemType { get; set; }
```

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

* enum [BarItemType](../../baritemtype/)
* class [BarStyle](../)
* namespace [Aspose.Tasks.Visualization](../../barstyle/)
* assembly [Aspose.Tasks](../../../)


