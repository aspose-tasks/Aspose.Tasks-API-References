---
title: "SaveTemplateOptions.RemoveBaselineValues"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Свойство SaveTemplateOptions. Получает или задает значение, указывающее, следует ли удалить все базовые значения из шаблона проекта."
type: docs
weight: 30
url: /ru/net/aspose.tasks.saving/savetemplateoptions/removebaselinevalues/
---
## SaveTemplateOptions.RemoveBaselineValues property

Получает или задает значение, указывающее, следует ли удалить все базовые значения из шаблона проекта.

```csharp
public bool RemoveBaselineValues { get; set; }
```

## Примеры

Показывает, как сохранить проект как шаблон, используя параметры.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");
var projectFileInfo = Project.GetProjectFileInfo(DataDir + "EstimatedMilestoneTasks.mpp");

Console.WriteLine("Project File Format: " + projectFileInfo.ProjectFileFormat);

// создать параметры сохранения шаблона
// и настроить его свойства
var options = new SaveTemplateOptions
{
    // установить значение, указывающее, следует ли удалить все фиксированные затраты из шаблона проекта
    RemoveFixedCosts = true,

    // установить значение, указывающее, следует ли удалить все фактические значения из шаблона проекта
    RemoveActualValues = true,

    // установить значение, указывающее, следует ли удалить ставки ресурсов из шаблона проекта
    RemoveResourceRates = true,

    // установить значение, указывающее, следует ли удалить все базовые значения из шаблона проекта
    RemoveBaselineValues = true
};

project.SaveAsTemplate(OutDir + "SaveProjectDataAsTemplate_out.mpt", options);

var templateFileInfo = Project.GetProjectFileInfo(DataDir + "SaveProjectDataAsTemplate_out.mpt");
Console.WriteLine("Project File Format: " + templateFileInfo.ProjectFileFormat);
```

### См. также

* class [SaveTemplateOptions](../)
* namespace [Aspose.Tasks.Saving](../../savetemplateoptions/)
* assembly [Aspose.Tasks](../../../)


