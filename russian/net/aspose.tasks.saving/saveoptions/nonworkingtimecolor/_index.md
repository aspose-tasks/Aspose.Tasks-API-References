---
title: "SaveOptions.NonWorkingTimeColor"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Свойство SaveOptions. Получает или задает цвет нерабочего времени"
type: docs
weight: 110
url: /ru/net/aspose.tasks.saving/saveoptions/nonworkingtimecolor/
---
## SaveOptions.NonWorkingTimeColor property

Получает или задает цвет нерабочего времени.

```csharp
public Color NonWorkingTimeColor { get; set; }
```

## Примеры

Показывает, как задать пользовательский цвет для нерабочего времени.

```csharp
var project = new Project(DataDir + "ReadCurrencyProperties.mpp");
SaveOptions options = new PdfSaveOptions { NonWorkingTimeColor = Color.LightGray };
project.Save(OutDir + "ReadCurrencyProperties_out.pdf", options);
```

### См. также

* class [SaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../saveoptions/)
* assembly [Aspose.Tasks](../../../)


