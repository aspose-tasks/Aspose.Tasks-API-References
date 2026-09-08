---
title: "PrimaveraSaveOptions.ActivityIdIncrement"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Свойство PrimaveraSaveOptions. Получает или задает инкремент, используемый при перенумерации идентификаторов действий"
type: docs
weight: 20
url: /ru/net/aspose.tasks.saving/primaverasaveoptions/activityidincrement/
---
## PrimaveraSaveOptions.ActivityIdIncrement property

Получает или задает приращение, используемое при перенумерации идентификаторов задач.

```csharp
public int ActivityIdIncrement { get; set; }
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


