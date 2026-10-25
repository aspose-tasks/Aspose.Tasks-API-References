---
title: "XpsOptions.RenderMetafileAsBitmap"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Свойство XpsOptions. Возвращает или задает значение, указывающее, следует ли отображать метафайл как растровое изображение."
type: docs
weight: 20
url: /ru/net/aspose.tasks.saving/xpsoptions/rendermetafileasbitmap/
---
## XpsOptions.RenderMetafileAsBitmap property

Получает или задает значение, указывающее, следует ли рендерить метафайл как растровое изображение.

```csharp
public bool RenderMetafileAsBitmap { get; set; }
```

## Примеры

Показывает, как сохранить проект в файл XPS.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

// создать параметры сохранения XPS и настроить параметры
var options = new XpsOptions
{
    RenderMetafileAsBitmap = true
};

project.Save(OutDir + "UseSvgOptions_out.xps", options);
```

### См. также

* class [XpsOptions](../)
* namespace [Aspose.Tasks.Saving](../../xpsoptions/)
* assembly [Aspose.Tasks](../../../)


