---
title: "Delege TaskBarTextConverter"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Görev verilerini çubuk metnine dönüştüren özel dönüştürücü"
type: docs
weight: 3380
url: /tr/net/aspose.tasks.visualization/taskbartextconverter/
---
## TaskBarTextConverter delegate

Görev verisinin çubuk metnine özel dönüştürücüsü.

```csharp
public delegate string TaskBarTextConverter(Task task);
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| görev | Görev | Görev çubuğu metninin oluşturulacağı görev. |

### Dönüş Değeri

Belirtilen görevle ilişkili çubuk için oluşturulacak metin.

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

* class [Task](../../aspose.tasks/task/)
* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


