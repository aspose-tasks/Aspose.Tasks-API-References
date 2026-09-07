---
title: "Enum GanttBarFillPattern"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Aspose.Tasks.Visualization.GanttBarFillPattern enum. Pola isi bentuk."
type: docs
weight: 3040
url: /id/net/aspose.tasks.visualization/ganttbarfillpattern/
---
## GanttBarFillPattern enumeration

Polanya pengisian sebuah bentuk.

```csharp
public enum GanttBarFillPattern
```

### Nilai

| Nama | Nilai | Deskripsi |
| --- | --- | --- |
| Hollow | `0` | Pola berongga. |
| SolidFill | `1` | Pola isi padat. |
| LightFill | `2` | Pola isi ringan. |
| MediumFill | `3` | Pola isi sedang. |
| DarkFill | `4` | Pola isi gelap. |
| DiagonalLeft | `5` | Pola diagonal kiri (dari kiri atas ke kanan bawah). |
| DiagonalRight | `6` | Pola diagonal kanan (dari kanan atas ke kiri bawah). |
| DiagonalCross | `7` | Pola diagonal silang. |
| LineVertical | `8` | Pola garis vertikal. |
| LineHorizontal | `9` | Pola garis horizontal. |
| LineCross | `10` | Pola garis silang. |
| SolidFillWithDashedBorder | `11` | Pola padat dengan batas putus-putus. |

## Contoh

Menampilkan cara mengatur gaya bar khusus pada tampilan proyek Gantt Chart.

```csharp
public void ImplementCustomBarStyle()
{
    try
    {
        var project = new Project(DataDir + "Blank2010.mpp");
        project.RootTask.Children.Add("Task");

        var view = (GanttChartView)project.DefaultView;
        var custom = GetCustomBarStyle();

        // Tambahkan gaya bar khusus ke koleksi bar khusus pada tampilan proyek
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

### Lihat Juga

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


