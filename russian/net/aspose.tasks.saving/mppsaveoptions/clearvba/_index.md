---
title: "MPPSaveOptions.ClearVba"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Свойство MPPSaveOptions. Возвращает или задает значение, указывающее, следует ли удалять существующие данные макросов VBA при сохранении проекта в формат MPP."
type: docs
weight: 20
url: /ru/net/aspose.tasks.saving/mppsaveoptions/clearvba/
---
## MPPSaveOptions.ClearVba property

Получает или задает значение, указывающее, следует ли удалять существующие данные макросов VBA при сохранении проекта в формат MPP.

```csharp
public bool ClearVba { get; set; }
```

## Примеры

Показывает, как удалить макросы VBA из файла MPP.

```csharp
var project = new Project(DataDir + "VbaProject.mpp");
project.Save(OutDir + "Vba.cleared.mpp", new MPPSaveOptions() { ClearVba = true });
```

### См. также

* class [MPPSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../mppsaveoptions/)
* assembly [Aspose.Tasks](../../../)


