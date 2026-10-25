---
title: "GanttBarStyle.LeftBarTextConverter"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "GanttBarStyle özelliği. Görev çubuğunun sol tarafında görüntülenecek metni elde etmek için kullanıcı tanımlı dönüştürücüyü alır veya ayarlar. LeftField özelliğinin değerini geçersiz kılar. MPP formatına kaydedilmez"
type: docs
weight: 100
url: /tr/net/aspose.tasks.visualization/ganttbarstyle/leftbartextconverter/
---
## GanttBarStyle.LeftBarTextConverter property

Görev çubuğunun sol tarafında görüntülenecek metni elde etmek için kullanıcı tanımlı dönüştürücüyü alır veya ayarlar. [`LeftField`](../leftfield/) özelliğinin değerini geçersiz kılar. MPP formatına kaydedilmez.

```csharp
public TaskBarTextConverter LeftBarTextConverter { get; set; }
```

## Örnekler

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

* delegate [TaskBarTextConverter](../../taskbartextconverter/)
* class [GanttBarStyle](../)
* namespace [Aspose.Tasks.Visualization](../../ganttbarstyle/)
* assembly [Aspose.Tasks](../../../)


