---
title: "ProjectView.GetDefaultGanttChartView"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "ProjectView yöntemi. id göstergeleri, ad, süre, başlangıç ve bitiş görev sütunlarını içerir."
type: docs
weight: 30
url: /tr/net/aspose.tasks.visualization/projectview/getdefaultganttchartview/
---
## ProjectView.GetDefaultGanttChartView method

id, göstergeler, ad, süre, başlangıç ve bitiş görev sütunlarını içerir.

```csharp
public static ProjectView GetDefaultGanttChartView()
```

### Dönüş Değeri

bir görünüm, [`GanttChartColumn`](../../ganttchartcolumn/) listesini içerir.

## Örnekler

Gantt şeması görünümüyle bir projenin nasıl kaydedileceğini gösterir.

```csharp
var project = new Project(DataDir + "Project2.mpp");
SaveOptions options = new PdfSaveOptions
{
    Timescale = Timescale.Months,
    View = ProjectView.GetDefaultGanttChartView()
};

project.Save(OutDir + "WorkWithProjectView_GanttChartView_out.pdf", options);
```

### Ayrıca Bakınız

* class [ProjectView](../)
* namespace [Aspose.Tasks.Visualization](../../projectview/)
* assembly [Aspose.Tasks](../../../)


