---
title: "FontResolveCallback"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Получает или задает обратный вызов, который можно использовать для настройки разрешённых шрифтов."
type: docs
weight: 60
url: /ru/net/aspose.tasks.saving/pdfsaveoptions/fontresolvecallback/
---
## PdfSaveOptions.FontResolveCallback property

Получает или задает обратный вызов, который можно использовать для настройки разрешённых шрифтов.

```csharp
public FontResolveCallbackDelegate FontResolveCallback { get; set; }
```

### Примеры

Показывает, как установить пользовательский обратный вызов разрешения шрифтов для выполнения пользовательского кода, задающего резервный шрифт или заменяющего конкретный шрифт.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

var options = new PdfSaveOptions
{
    PresentationFormat = PresentationFormat.GanttChart,
    FontResolveCallback = delegate(FontResolveEventArgs args)
    {
        if (args.RequestedFontName != args.ResolvedFontName)
        {
            // Похоже, точный шрифт не найден, и был установлен резервный шрифт.
            // Мы можем переопределить резервный шрифт.
            args.ResolvedFontName = "Arial";
        }

        // Или просто заменить конкретный шрифт:
        if (args.RequestedFontName == "Comic Sans MS")
        {
            args.ResolvedFontName = "Arial";
        }
    }
};

project.Save(OutDir + "EstimatedMilestoneTasks_out3.pdf", options);
```

### См. также

* delegate [FontResolveCallbackDelegate](../../../aspose.tasks/fontresolvecallbackdelegate)
* class [PdfSaveOptions](../../pdfsaveoptions)
* namespace [Aspose.Tasks.Saving](../../pdfsaveoptions)
* assembly [Aspose.Tasks](../../../)

<!-- НЕ РЕДАКТИРОВАТЬ: сгенерировано xmldocmd для Aspose.Tasks.dll -->
