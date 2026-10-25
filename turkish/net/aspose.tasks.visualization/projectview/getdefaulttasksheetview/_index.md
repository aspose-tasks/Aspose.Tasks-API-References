---
title: "ProjectView.GetDefaultTaskSheetView"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "ProjectView yöntemi. id göstergeleri, ad, süre, başlangıç, bitiş, öncüller ve kaynak adları görev sütunlarını içerir."
type: docs
weight: 60
url: /tr/net/aspose.tasks.visualization/projectview/getdefaulttasksheetview/
---
## ProjectView.GetDefaultTaskSheetView method

id, göstergeler, ad, süre, başlangıç, bitiş, öncüller ve kaynak adları görev sütunlarını içerir.

```csharp
public static ProjectView GetDefaultTaskSheetView()
```

### Dönüş Değeri

bir görünüm, [`GanttChartColumn`](../../ganttchartcolumn/) listesini içerir.

## Örnekler

Görev sayfası görünümüyle bir projenin nasıl kaydedileceğini gösterir.

```csharp
var project = new Project(DataDir + "Project2.mpp");
SaveOptions options = new PdfSaveOptions
{
    Timescale = Timescale.Months,
    View = ProjectView.GetDefaultTaskSheetView()
};

project.Save(OutDir + "WorkWithProjectView_TaskSheetView_out.pdf", options);
```

### Ayrıca Bakınız

* class [ProjectView](../)
* namespace [Aspose.Tasks.Visualization](../../projectview/)
* assembly [Aspose.Tasks](../../../)


