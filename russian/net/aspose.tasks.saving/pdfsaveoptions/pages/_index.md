---
title: "PdfSaveOptions.Pages"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Свойство PdfSaveOptions. Получает или задает список номеров страниц для сохранения при сохранении макета проекта в отдельные файлы. Если список пуст, будут сохранены все страницы."
type: docs
weight: 60
url: /ru/net/aspose.tasks.saving/pdfsaveoptions/pages/
---
## PdfSaveOptions.Pages property

Получает или задает список номеров страниц для сохранения при сохранении макета проекта в отдельные файлы. Если список пуст, будут сохранены все страницы.

```csharp
public List<int> Pages { get; set; }
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


