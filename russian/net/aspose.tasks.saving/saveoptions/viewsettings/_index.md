---
title: "SaveOptions.ViewSettings"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Свойство SaveOptions. Получает или задает представление View для рендеринга. Вы можете использовать эту опцию, чтобы явно указать, какое представление следует сохранять в форматы PDF, HTML или Image. Если это свойство задано, свойство PresentationFormat игнорируется при сохранении проекта. Представление должно быть одним из следующих экранов Screen: Gantt, TaskSheet, TaskUsage, ResourceSheet, ResourceUsage."
type: docs
weight: 240
url: /ru/net/aspose.tasks.saving/saveoptions/viewsettings/
---
## SaveOptions.ViewSettings property

Получает или задает представление ([`View`](../view/)) для рендеринга. Вы можете использовать эту опцию, чтобы явно указать, какое представление следует сохранять в форматы PDF, HTML или Image. Если это свойство задано, свойство [`PresentationFormat`](../../../aspose.tasks.visualization/presentationformat/) игнорируется при сохранении проекта. Представление должно быть одним из следующих экранов (([`Screen`](../../../aspose.tasks/view/screen/))): (Gantt, TaskSheet, TaskUsage, ResourceSheet, ResourceUsage).

```csharp
public View ViewSettings { get; set; }
```

### Исключения

| исключение | условие |
| --- | --- |
| ArgumentException | Когда вызывается метод set и предоставлен экземпляр класса View с неподдерживаемым значением свойства Screen. |

## Примеры

Показано, как использовать 'SaveOptions.ViewSettings' для указания представления, которое должно быть отрендерено в PDF.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

var view = project.Views.First(v => v.Screen == ViewScreen.Gantt);
Console.WriteLine("Page size specified in view settings: " + view.PageInfo.PageSettings.PaperSize);
Console.WriteLine("Page orientation: {0}", view.PageInfo.PageSettings.IsPortrait ? "Portrait" : "Landscape");

PdfSaveOptions saveOptions = new PdfSaveOptions();
saveOptions.PageSize = PageSize.DefinedInView;
saveOptions.Timescale = Timescale.DefinedInView;
saveOptions.StartDate = new DateTime(2012, 12, 22);
saveOptions.EndDate = new DateTime(2013, 05, 10);
saveOptions.ViewSettings = view;

project.Save(OutDir + "SaveToPdfUsingSpecificView_out.pdf", saveOptions);
```

### См. также

* class [View](../../../aspose.tasks/view/)
* class [SaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../saveoptions/)
* assembly [Aspose.Tasks](../../../)


