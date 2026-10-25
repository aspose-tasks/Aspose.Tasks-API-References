---
title: "XpsOptions.XpsOptions"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Конструктор XpsOptions. Инициализирует новый экземпляр класса XpsOptions"
type: docs
weight: 10
url: /ru/net/aspose.tasks.saving/xpsoptions/xpsoptions/
---
## XpsOptions constructor

Инициализирует новый экземпляр класса [`XpsOptions`](../).

```csharp
public XpsOptions()
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


