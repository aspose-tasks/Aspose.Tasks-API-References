---
title: "Class SaveTemplateOptions"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Aspose.Tasks.Saving.SaveTemplateOptions class. Позволяет указать дополнительные параметры при сохранении проекта в виде шаблона"
type: docs
weight: 2200
url: /ru/net/aspose.tasks.saving/savetemplateoptions/
---
## SaveTemplateOptions class

Позволяет указать дополнительные параметры при сохранении проекта в виде шаблона.

```csharp
public class SaveTemplateOptions
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [SaveTemplateOptions](savetemplateoptions/)() | Конструктор по умолчанию. |

## Свойства

| Имя | Описание |
| --- | --- |
| [RemoveActualValues](../../aspose.tasks.saving/savetemplateoptions/removeactualvalues/) { get; set; } | Получает или задает значение, указывающее, следует ли удалить все фактические значения из шаблона проекта. |
| [RemoveBaselineValues](../../aspose.tasks.saving/savetemplateoptions/removebaselinevalues/) { get; set; } | Получает или задает значение, указывающее, следует ли удалить все базовые значения из шаблона проекта. |
| [RemoveFixedCosts](../../aspose.tasks.saving/savetemplateoptions/removefixedcosts/) { get; set; } | Получает или задает значение, указывающее, следует ли удалить все фиксированные затраты из шаблона проекта. |
| [RemoveResourceRates](../../aspose.tasks.saving/savetemplateoptions/removeresourcerates/) { get; set; } | Получает или задает значение, указывающее, следует ли удалить ставки ресурсов из шаблона проекта. |

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

* namespace [Aspose.Tasks.Saving](../../aspose.tasks.saving/)
* assembly [Aspose.Tasks](../../)


