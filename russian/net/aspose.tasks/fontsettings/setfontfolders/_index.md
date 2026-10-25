---
title: "FontSettings.SetFontFolders"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Метод FontSettings. Устанавливает папки, в которых Aspose.Tasks ищет шрифты TrueType при рендеринге представления проектов"
type: docs
weight: 50
url: /ru/net/aspose.tasks/fontsettings/setfontfolders/
---
## FontSettings.SetFontFolders method

Задает папки, в которых Aspose.Tasks ищет TrueType‑шрифты при рендеринге представления проекта.

```csharp
public void SetFontFolders(string[] fontFolders, bool recursive)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| fontFolders | String[] | Массив папок, содержащих шрифты TrueType. |
| recursive | Boolean | Если true, указанные папки будут просканированы рекурсивно. |

## Примеры

Показывает, как установить пользовательскую папку шрифтов.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

var options = new PdfSaveOptions
{
    PresentationFormat = PresentationFormat.GanttChart,
};

// Файлы шрифтов TrueType для всех шрифтов, используемых в открытом проекте, должны находиться в папке MyFonts.
options.FontSettings.SetFontFolders(new string[] { "c:\\MyFonts"}, true);

project.Save(OutDir + "EstimatedMilestoneTasks_out4.pdf", options);
```

### См. также

* class [FontSettings](../)
* namespace [Aspose.Tasks](../../fontsettings/)
* assembly [Aspose.Tasks](../../../)


