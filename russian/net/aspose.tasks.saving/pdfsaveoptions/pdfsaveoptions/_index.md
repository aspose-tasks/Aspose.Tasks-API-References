---
title: "PdfSaveOptions.PdfSaveOptions"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Конструктор PdfSaveOptions. Инициализирует новый экземпляр класса PdfSaveOptions, который можно использовать для сохранения документа в формате PDF."
type: docs
weight: 10
url: /ru/net/aspose.tasks.saving/pdfsaveoptions/pdfsaveoptions/
---
## PdfSaveOptions constructor

Инициализирует новый экземпляр класса [`PdfSaveOptions`](../), который можно использовать для сохранения документа в формате [`PDF`](../../savefileformat/).

```csharp
public PdfSaveOptions()
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

* class [PdfSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../pdfsaveoptions/)
* assembly [Aspose.Tasks](../../../)


