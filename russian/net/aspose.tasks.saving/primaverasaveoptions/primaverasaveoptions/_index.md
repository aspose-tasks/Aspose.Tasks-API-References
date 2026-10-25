---
title: "PrimaveraSaveOptions.PrimaveraSaveOptions"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Конструктор PrimaveraSaveOptions. Инициализирует новый экземпляр класса PrimaveraSaveOptions"
type: docs
weight: 10
url: /ru/net/aspose.tasks.saving/primaverasaveoptions/primaverasaveoptions/
---
## PrimaveraSaveOptions constructor

Инициализирует новый экземпляр класса [`PrimaveraSaveOptions`](../).

```csharp
public PrimaveraSaveOptions()
```

## Примеры

Показывает, как работать с &lt;see cref=\"Aspose.Tasks.Saving.PrimaveraSaveOptions\" /&gt;.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

// создайте параметры сохранения Primavera и настройте их
var options = new PrimaveraSaveOptions
                  {
                      // определите префикс и суффикс активности
                      ActivityIdPrefix = "TEST",
                      ActivityIdSuffix = 10000,

                      // контролируйте перенумерацию задач
                      ActivityIdIncrement = 5,
                      RenumberActivityIds = true
                  };

project.Save(OutDir + "WorkWithPrimaveraSaveOptions_out.xer", options);
```

### См. также

* class [PrimaveraSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../primaverasaveoptions/)
* assembly [Aspose.Tasks](../../../)


