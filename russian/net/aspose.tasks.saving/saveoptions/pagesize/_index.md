---
title: "SaveOptions.PageSize"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Свойство SaveOptions. Получает или задает размер страницы для рендеринга. Значение по умолчанию — PageSize.A4"
type: docs
weight: 130
url: /ru/net/aspose.tasks.saving/saveoptions/pagesize/
---
## SaveOptions.PageSize property

Получает или задает размер страницы для рендеринга (значение по умолчанию — PageSize.A4).

```csharp
public PageSize PageSize { get; set; }
```

## Примеры

Показывает, как установить размер страницы (может быть одним из значений перечисления &lt;see cref="P:Aspose.Tasks.Visualization.TiffCompression" /&gt;).

```csharp
var project = new Project(DataDir + "Project2.mpp");

const PresentationFormat format = PresentationFormat.GanttChart;

// Отрендерить проект во всех предопределённых размерах страниц
foreach (var pageSize in (PageSize[])Enum.GetValues(typeof(PageSize)))
{
    var options = new PdfSaveOptions
    {
        PresentationFormat = format,
        FitContent = true,
        PageSize = pageSize
    };
    project.Save(OutDir + "PredefinedPageSizes_" + format + "_" + pageSize + "_out.pdf", options);
}
```

### См. также

* enum [PageSize](../../../aspose.tasks.visualization/pagesize/)
* class [SaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../saveoptions/)
* assembly [Aspose.Tasks](../../../)


