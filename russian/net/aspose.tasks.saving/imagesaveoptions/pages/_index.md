---
title: "ImageSaveOptions.Pages"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Свойство ImageSaveOptions. Получает или задает список номеров страниц для сохранения при экспорте макета проекта в отдельные файлы. Все страницы будут сохранены, если этот список пуст."
type: docs
weight: 50
url: /ru/net/aspose.tasks.saving/imagesaveoptions/pages/
---
## ImageSaveOptions.Pages property

Получает или задает список номеров страниц для сохранения при сохранении макета проекта в отдельные файлы. Если список пуст, будут сохранены все страницы.

```csharp
public List<int> Pages { get; set; }
```

## Примеры

Показывает, как сохранить выбранные страницы в виде изображения.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

var options = new ImageSaveOptions(SaveFileFormat.Jpeg)
                  {
                      RenderToSinglePage = false,
                      StartDate = project.Get(Prj.StartDate),
                      EndDate = project.Get(Prj.FinishDate),
                      PageSize = PageSize.Letter
                  };
options.Pages.Add(2);

project.Save(OutDir + "SaveSelectedPagesImageSaveOptions_page2_out.jpeg", options);
```

### См. также

* class [ImageSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../imagesaveoptions/)
* assembly [Aspose.Tasks](../../../)


