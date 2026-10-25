---
title: "Enum GanttBarEndShape"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Aspose.Tasks.Visualization.GanttBarEndShape enum. Çubuklarda ve ilerleme çizgilerindeki ilerleme noktalarında uç şekli temsil eder"
type: docs
weight: 3030
url: /tr/net/aspose.tasks.visualization/ganttbarendshape/
---
## GanttBarEndShape enumeration

Çubuklarda ve ilerleme çizgilerindeki ilerleme noktalarında son şekli temsil eder.

```csharp
public enum GanttBarEndShape
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| ArrowDown | `14` | Aşağı yön gösteren ok Gantt çubuğu uç şekli. |
| ArrowUp | `8` | Yukarı yön gösteren ok Gantt çubuğu uç şekli. |
| CaretDownTop | `9` | Çubuğun üst yarısında aşağı yön gösteren işaret Gantt çubuğu uç şekli. |
| CaretUpBottom | `10` | Çubuğun alt yarısında yukarı yön gösteren işaret Gantt çubuğu uç şekli. |
| Circle | `19` | Daire Gantt çubuğu uç şekli gösterir. |
| CircleArrowDown | `18` | Aşağı yön gösteren daire içinde ok Gantt çubuğu uç şekli. |
| CircleArrowUp | `17` | Yukarı yön gösteren daire içinde ok Gantt çubuğu uç şekli. |
| CircleDiamond | `13` | Daire içinde elmas Gantt çubuğu uç şekli. |
| CircleTriangleDown | `16` | Aşağı yön gösteren daire içinde üçgen Gantt çubuğu uç şekli. |
| CircleTriangleUp | `15` | Yukarı yön gösteren daire içinde üçgen Gantt çubuğu uç şekli. |
| Diamond | `3` | Elmas Gantt çubuğu uç şekli. |
| HouseDown | `2` | Baş aşağı ev Gantt çubuğu uç şekli. |
| HouseUp | `1` | Ev Gantt çubuğu uç şekli. |
| LeftBracket | `21` | Sol köşeli parantez Gantt çubuğu uç şekli. |
| LeftFade | `23` | Sol solma Gantt çubuğu uç şekli. |
| LineShape | `11` | Çizgi Gantt çubuğu uç şekli. |
| NoBarEndShape | `0` | Hiçbiri Gantt çubuğu uç şekli. |
| RightBracket | `22` | Sağ köşeli parantez Gantt çubuğu uç şekli. |
| RightFade | `24` | Sağ solma Gantt çubuğu uç şekli. |
| Square | `12` | Kare Gantt çubuğu uç şekli. |
| Star | `20` | Yıldız Gantt çubuğu uç şekli. |
| TriangleDown | `5` | Aşağı yön gösteren üçgen Gantt çubuğu uç şekli. |
| TriangleLeft | `7` | Sol yön gösteren üçgen Gantt çubuğu uç şekli gösterir. |
| TriangleRight | `6` | Sağ yön gösteren üçgen Gantt çubuğu uç şekli gösterir. |
| TriangleUp | `4` | Yukarı yön gösteren daire içinde üçgen Gantt çubuğu uç şekli. |

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


