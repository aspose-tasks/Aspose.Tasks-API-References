---
title: "Απαρίθμηση GanttBarFillPattern"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Aspose.Tasks.Visualization.GanttBarFillPattern enum. Ένα μοτίβο γεμίσματος σχήματος"
type: docs
weight: 3040
url: /el/net/aspose.tasks.visualization/ganttbarfillpattern/
---
## GanttBarFillPattern enumeration

Μοτίβο γεμίσματος ενός σχήματος.

```csharp
public enum GanttBarFillPattern
```

### Τιμές

| Όνομα | Τιμή | Περιγραφή |
| --- | --- | --- |
| Hollow | `0` | Κενό μοτίβο. |
| SolidFill | `1` | Συμπαγές μοτίβο γεμίσματος. |
| LightFill | `2` | Ανοιχτό μοτίβο γεμίσματος. |
| MediumFill | `3` | Μεσαίο μοτίβο γεμίσματος. |
| DarkFill | `4` | Σκούρο μοτίβο γεμίσματος. |
| DiagonalLeft | `5` | Διαγώνιο αριστερό μοτίβο (από το πάνω αριστερό στο κάτω δεξί). |
| DiagonalRight | `6` | Διαγώνιο δεξιό μοτίβο (από το πάνω δεξιό στο κάτω αριστερό). |
| DiagonalCross | `7` | Διαγώνιο σταυροειδές μοτίβο. |
| LineVertical | `8` | Κατακόρυφο μοτίβο γραμμής. |
| LineHorizontal | `9` | Οριζόντιο μοτίβο γραμμής. |
| LineCross | `10` | Σταυροειδές μοτίβο γραμμής. |
| SolidFillWithDashedBorder | `11` | Συμπαγές με διακεκομμένο περίγραμμα μοτίβο. |

## Παραδείγματα

Δείχνει πώς να ορίσετε προσαρμοσμένα στυλ μπάρας στην προβολή έργου Gantt Chart.

```csharp
public void ImplementCustomBarStyle()
{
    try
    {
        var project = new Project(DataDir + "Blank2010.mpp");
        project.RootTask.Children.Add("Task");

        var view = (GanttChartView)project.DefaultView;
        var custom = GetCustomBarStyle();

        // Προσθέστε το προσαρμοσμένο στυλ μπάρας στη συλλογή προσαρμοσμένων μπαρών της προβολής έργου
        view.CustomBarStyles.Add(custom);

        SimpleSaveOptions options = new MPPSaveOptions
        {
            WriteViewData = true
        };

        project.Save(OutDir + "ImplementCustomBarStyleWriting_out.mpp", options);
    }
    catch (NotSupportedException ex)
    {
        Console.WriteLine(
            ex.Message
            + "\nThis example will only work if you apply a valid Aspose License. You can purchase full license or get 30 day temporary license from http://www.aspose.com/purchase/default.aspx.");
    }
}

public static GanttBarStyle GetCustomBarStyle()
{
    var style = new GanttBarStyle
    {
        ShowForTaskUid = 1,
        MiddleShape = GanttBarMiddleShape.RectangleBottom,
        MiddleFillPattern = GanttBarFillPattern.MediumFill,
        MiddleShapeColor = Color.Blue,

        StartShape = GanttBarEndShape.ArrowDown,
        StartShapeColor = Color.Red,

        EndShape = GanttBarEndShape.ArrowUp,
        EndShapeColor = Color.Yellow,

        LeftField = Field.TaskResourceNames,
        RightField = Field.TaskName,
        TopField = Field.TaskStart,
        BottomField = Field.TaskFinish,
        InsideField = Field.TaskDuration
    };

    return style;
}
```

### Δείτε επίσης

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


