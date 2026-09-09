---
title: "Enum GanttBarFillPattern"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Aspose.Tasks.Visualization.GanttBarFillPattern enum. Bir şeklin dolgu deseni"
type: docs
weight: 3040
url: /tr/net/aspose.tasks.visualization/ganttbarfillpattern/
---
## GanttBarFillPattern enumeration

Bir şeklin doldurma deseni.

```csharp
public enum GanttBarFillPattern
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| Hollow | `0` | Boş desen. |
| SolidFill | `1` | Katı dolgu deseni. |
| LightFill | `2` | Açık dolgu deseni. |
| MediumFill | `3` | Orta dolgu deseni. |
| DarkFill | `4` | Koyu dolgu deseni. |
| DiagonalLeft | `5` | Sol çapraz desen (sol üstten sağ alta). |
| DiagonalRight | `6` | Sağ çapraz desen (sağ üstten sol alta). |
| DiagonalCross | `7` | Diyagonal çapraz desen. |
| LineVertical | `8` | Dikey çizgi deseni. |
| LineHorizontal | `9` | Yatay çizgi deseni. |
| LineCross | `10` | Çapraz çizgi deseni. |
| SolidFillWithDashedBorder | `11` | Kesikli kenarlı katı desen. |

## Örnekler

Gantt Şeması proje görünümünün özel çubuk stillerinin nasıl ayarlanacağını gösterir.

```csharp
public void ImplementCustomBarStyle()
{
    try
    {
        var project = new Project(DataDir + "Blank2010.mpp");
        project.RootTask.Children.Add("Task");

        var view = (GanttChartView)project.DefaultView;
        var custom = GetCustomBarStyle();

        // Özel çubuk stilini proje görünümünün özel çubuk koleksiyonuna ekleyin
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

### Ayrıca Bakınız

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


