---
title: "SaveOptions.FitContent"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Свойство SaveOptions. Получает или задает значение, указывающее, следует ли увеличивать высоту строки, чтобы она соответствовала её содержимому."
type: docs
weight: 50
url: /ru/net/aspose.tasks.saving/saveoptions/fitcontent/
---
## SaveOptions.FitContent property

Получает или задает значение, указывающее, следует ли увеличивать высоту строки, чтобы она соответствовала содержимому.

```csharp
public bool FitContent { get; set; }
```

## Примеры

Показывает, как установить параметр, увеличивать ли высоту строки, чтобы она соответствовала содержимому.

```csharp
var project = new Project(DataDir + "CreateProject2.mpp");
SaveOptions options = new PdfSaveOptions
{
    // Установить параметр fit content в значение true
    FitContent = true,
    Timescale = Timescale.Months,
    PresentationFormat = PresentationFormat.TaskUsage
};
project.Save(OutDir + "FitContentsToCellSize_out.pdf", options);
```

### См. также

* class [SaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../saveoptions/)
* assembly [Aspose.Tasks](../../../)


