---
title: "Класс PrimaveraXmlSaveOptions"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Класс Aspose.Tasks.Saving.PrimaveraXmlSaveOptions. Позволяет указать дополнительные параметры при сохранении проекта в формат Primavera XML."
type: docs
weight: 2160
url: /ru/net/aspose.tasks.saving/primaveraxmlsaveoptions/
---
## PrimaveraXmlSaveOptions class

Позволяет указать дополнительные параметры при сохранении проекта в формат Primavera XML.

```csharp
public class PrimaveraXmlSaveOptions : SimpleSaveOptions
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [PrimaveraXmlSaveOptions](primaveraxmlsaveoptions/)() | Инициализирует новый экземпляр класса `PrimaveraXmlSaveOptions`. |

## Свойства

| Имя | Описание |
| --- | --- |
| [SaveFormat](../../aspose.tasks.saving/simplesaveoptions/saveformat/) { get; } | Получает или задает формат, в котором будет сохраняться документ, если используется этот объект параметров сохранения. |
| [SaveRootTask](../../aspose.tasks.saving/primaveraxmlsaveoptions/saveroottask/) { get; set; } | Получает или задаёт значение, указывающее, сохранять корневую задачу или нет. |
| [SkipSummaryAssignments](../../aspose.tasks.saving/primaveraxmlsaveoptions/skipsummaryassignments/) { get; set; } | Получает или задаёт значение, указывающее, следует ли пропускать назначения ресурсов к сводным задачам при экспорте. |
| [TasksComparer](../../aspose.tasks.saving/simplesaveoptions/taskscomparer/) { get; set; } | Получает или задает компаратор для сортировки задач на диаграмме Ганта и листе задач. |
| [TasksFilter](../../aspose.tasks.saving/simplesaveoptions/tasksfilter/) { get; set; } | Получает или задает условие, используемое для фильтрации задач, отрисованных на диаграммах Ганта, листе задач и использовании задач. |

## Примеры

Показывает, как экспортировать в файл Primavera XML.

```csharp
var project = new Project(DataDir + "project.xml");

var options = new PrimaveraXmlSaveOptions();
options.SaveRootTask = false;
project.Save(OutDir + "UsingPrimaveraXMLSaveOptions_out.xml", options);
```

### См. также

* class [SimpleSaveOptions](../simplesaveoptions/)
* namespace [Aspose.Tasks.Saving](../../aspose.tasks.saving/)
* assembly [Aspose.Tasks](../../)


