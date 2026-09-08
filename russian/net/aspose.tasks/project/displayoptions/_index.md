---
title: "Project.DisplayOptions"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Свойство Project. Получает экземпляр класса ProjectDisplayOptions"
type: docs
weight: 380
url: /ru/net/aspose.tasks/project/displayoptions/
---
## Project.DisplayOptions property

Получает экземпляр класса [`ProjectDisplayOptions`](../../projectdisplayoptions/).

```csharp
public ProjectDisplayOptions DisplayOptions { get; }
```

## Примеры

Показывает, как настроить параметры отображения проекта.

```csharp
var project = new Project(DataDir + "Blank2010.mpp");

// Задайте значение, указывающее, следует ли показывать предупреждения, когда Project обнаруживает возможный конфликт планирования с вручную запланированной задачей.
// Эта опция доступна в версии Project 2010 и позже.
project.DisplayOptions.ShowTaskScheduleWarnings = false;
```

### См. также

* class [ProjectDisplayOptions](../../projectdisplayoptions/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


