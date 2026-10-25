---
title: "Sınıf ProjectView"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Aspose.Tasks.Visualization.ProjectView sınıfı. Projeler görünüm sınıfı"
type: docs
weight: 3300
url: /tr/net/aspose.tasks.visualization/projectview/
---
## ProjectView class

Projenin görünüm sınıfı

```csharp
public class ProjectView
```

## Yapıcılar

| Ad | Açıklama |
| --- | --- |
| [ProjectView](projectview/)(IEnumerable&lt;ViewColumn&gt;) | Yeni bir `ProjectView` sınıfı örneği başlatır. |

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [Columns](../../aspose.tasks.visualization/projectview/columns/) { get; } | Proje görünüm sütunlarını alır. |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| static [GetDefaultAssignmentView](../../aspose.tasks.visualization/projectview/getdefaultassignmentview/)() | Uid, görev adı, kaynak adı, iş ve süre atama sütunlarını içerir. |
| static [GetDefaultGanttChartView](../../aspose.tasks.visualization/projectview/getdefaultganttchartview/)() | id, göstergeler, ad, süre, başlangıç ve bitiş görev sütunlarını içerir. |
| static [GetDefaultResourceSheetView](../../aspose.tasks.visualization/projectview/getdefaultresourcesheetview/)() | Uid, kaynak adı, tip, malzeme etiketi, baş harfler, grup, maksimum birimler, standart oran, fazla mesai oranı, kullanım başına maliyet, birikim zamanı, temel takvim ve kod kaynak sütunlarını içerir. |
| static [GetDefaultResourceUsageView](../../aspose.tasks.visualization/projectview/getdefaultresourceusageview/)() | Uid, ad, başlangıç, bitiş ve iş kaynağı sütunlarını içerir. |
| static [GetDefaultTaskSheetView](../../aspose.tasks.visualization/projectview/getdefaulttasksheetview/)() | id, göstergeler, ad, süre, başlangıç, bitiş, öncüller ve kaynak adları görev sütunlarını içerir. |

## Örnekler

Atama görünümüyle bir projenin nasıl kaydedileceğini gösterir.

```csharp
var project = new Project(DataDir + "Project2.mpp");
SaveOptions options = new PdfSaveOptions
{
    Timescale = Timescale.Months,
    View = ProjectView.GetDefaultAssignmentView()
};

project.Save(OutDir + "WorkWithProjectView_AssignmentView_out.pdf", options);
```

### Ayrıca Bakınız

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


