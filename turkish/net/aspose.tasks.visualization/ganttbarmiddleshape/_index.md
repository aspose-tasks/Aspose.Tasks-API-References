---
title: "Enum GanttBarMiddleShape"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Aspose.Tasks.Visualization.GanttBarMiddleShape enum. Bir çubuğun orta şeklini belirtir."
type: docs
weight: 3050
url: /tr/net/aspose.tasks.visualization/ganttbarmiddleshape/
---
## GanttBarMiddleShape enumeration

Bir çubuğun orta şeklini belirtir.

```csharp
public enum GanttBarMiddleShape
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| LineBottom | `7` | Alt hizalı çizgi şeklini gösterir. |
| LineMiddle | `6` | Ortaya hizalı çizgi şeklini gösterir. |
| LineTop | `5` | Üst hizalı çizgi şeklini gösterir. |
| None | `0` | Boş şekli gösterir. |
| RectangleBar | `1` | Tam yükseklikte dikdörtgen çubuk şeklini gösterir. |
| RectangleBottom | `4` | Alt hizalı yarı yükseklikte dikdörtgen çubuk şeklini gösterir. |
| RectangleMiddle | `3` | Merkez hizalı 1/3 yükseklikte dikdörtgen çubuk şeklini gösterir. |
| RectangleTop | `2` | Üst hizalı yarı yüksekliğinde dikdörtgen çubuk şeklini gösterir. |

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

Gantt Şeması görünümünün özel çubuk stillerinin nasıl kullanılacağını gösterir.

```csharp
var project = new Project(DataDir + "Project2.mpp");

var ganttChartView = (GanttChartView)project.Views.First(v => v.Name == "Gantt &Chart");
PdfSaveOptions saveOptions = new PdfSaveOptions();
saveOptions.Timescale = Timescale.DefinedInView;
saveOptions.ViewSettings = ganttChartView;

// Çubuk stilleri görev‑özel (GanttChartView.CustomBarStyles içinde bulunur) olabilir
// kategori‑özel (GanttChartView.BarStyles içinde bulunur)
foreach (GanttBarStyle ganttBarStyle in ganttChartView.CustomBarStyles)
{
    if (ganttBarStyle.ShowForTaskUid != 4)
    {
        continue;
    }

    // Demonstrasyon amacıyla, Benzersiz ID = 4 olan Görev için stili değiştiriyoruz
    // Burada alanı (TaskName) görev çubuğunun sol tarafına render edecek şekilde ayarlarız.
    ganttBarStyle.LeftField = Field.TaskName;
    // Burada, görev çubuğu içinde hangi metnin render edileceğini kontrol etmek için özel dönüştürücü ayarlarız.
    ganttBarStyle.InsideBarTextConverter = task => "Hours rem.: " + (int)task.Get(Tsk.RemainingWork).TimeSpan.TotalHours;

    ganttBarStyle.MiddleShapeColor = Color.Green;
    ganttBarStyle.MiddleShape = GanttBarMiddleShape.LineTop;
    ganttBarStyle.StartShape = GanttBarEndShape.LeftBracket;
    ganttBarStyle.StartShapeColor = Color.Aqua;
    ganttBarStyle.EndShape = GanttBarEndShape.RightBracket;
    ganttBarStyle.EndShapeColor = Color.Aquamarine;
}

foreach (GanttBarStyle ganttBarStyle in ganttChartView.BarStyles)
{
    if (!ganttBarStyle.ShowForCategories.Contains(GanttBarShowFor.Milestone))
    {
        continue;
    }

    // Demonstrasyon amacıyla, kilometre taşı görevlerine uygulanabilir stilleri değiştiriyoruz.

    ganttBarStyle.StartShape = GanttBarEndShape.Diamond;
    ganttBarStyle.RightField = Field.TaskActualFinish;
    ganttBarStyle.TopBarTextConverter = task => task.Get(Tsk.ActualStart).Day.ToString();
}

project.Save(OutDir + "WorkWithGanttChartViewBarStyles_out.pdf", saveOptions);
```

### Ayrıca Bakınız

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


