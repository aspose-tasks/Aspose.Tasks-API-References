---
title: "SaveOptions.PageCount"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Свойство SaveOptions. Получает или задает количество страниц проекта."
type: docs
weight: 120
url: /ru/net/aspose.tasks.saving/saveoptions/pagecount/
---
## SaveOptions.PageCount property

Получает или задает количество страниц проекта.

```csharp
public int PageCount { get; }
```

## Примеры

Показывает, как сохранить выбранные страницы проекта в PDF‑файл.

```csharp
var project = new Project(DataDir + "Software Development Plan.mpp");
var options = new PdfSaveOptions();
options.RenderToSinglePage = false;
options.Pages = new List<int>();

// проверим, сколько страниц можно экспортировать
Console.WriteLine("Page Count: " + options.PageCount);

options.Pages.Add(1);
options.Pages.Add(4);
project.Save(OutDir + "SaveToMultiplePDFFiles_out.pdf", options);
```

### См. также

* class [SaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../saveoptions/)
* assembly [Aspose.Tasks](../../../)


