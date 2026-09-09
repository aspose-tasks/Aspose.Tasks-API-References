---
title: "GanttChartView.TextStyles"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "GanttChartView özelliği. Gantt Şeması görünümünün TextStyle listesini alır veya ayarlar"
type: docs
weight: 170
url: /tr/net/aspose.tasks/ganttchartview/textstyles/
---
## GanttChartView.TextStyles property

Gantt Şeması görünümünün [`TextStyle`](../../../aspose.tasks.visualization/textstyle/) listesini alır veya ayarlar.

```csharp
public List<TextStyle> TextStyles { get; set; }
```

## Örnekler

Gantt şeması metin stillerinin nasıl okunacağını gösterir.

```csharp
var project = new Project(DataDir + "Project2.mpp");
project.Set(Prj.StatusDate, project.Get(Prj.StartDate));

var view = (GanttChartView)project.Views.ToList()[0];

// Gantt şeması görünümünün metin stilleri üzerinde yineleme yapın
foreach (var style in view.TextStyles)
{
    Console.WriteLine("Style Item Type: " + style.ItemType);
    Console.WriteLine("Style Font name: " + style.Font.FontFamily);
    Console.WriteLine();
}
```

### Ayrıca Bakınız

* class [TextStyle](../../../aspose.tasks.visualization/textstyle/)
* class [GanttChartView](../)
* namespace [Aspose.Tasks](../../ganttchartview/)
* assembly [Aspose.Tasks](../../../)


