---
title: "PrimaveraSaveOptions.SkipSummaryAssignments"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Свойство PrimaveraSaveOptions. Получает или задает значение, указывающее, следует ли пропускать назначения ресурсов к сводным задачам при экспорте"
type: docs
weight: 60
url: /ru/net/aspose.tasks.saving/primaverasaveoptions/skipsummaryassignments/
---
## PrimaveraSaveOptions.SkipSummaryAssignments property

Получает или задаёт значение, указывающее, следует ли пропускать назначения ресурсов к сводным задачам при экспорте.

```csharp
public bool SkipSummaryAssignments { get; set; }
```

## Примечания

Программное обеспечение Primavera не поддерживает назначения ресурсов к сводным (WBS) задачам. Поэтому экспорт таких назначений может привести к созданию недействительного файла согласно модели Primavera. Если true, назначения к сводным задачам пропускаются при экспорте. Если false (значение по умолчанию), будет выброшено исключение, если во время экспорта будет обнаружено назначение к сводной задаче.

## Примеры

Показывает, как использовать флаг SkipSummaryAssignments.

```csharp
var project = new Project(DataDir + "Blank2010.mpp");

var resource = project.Resources.Add("Resource");

var summaryTask = project.RootTask.Children.Add("Summary");
summaryTask.Children.Add("Task");

// Primavera не поддерживает назначения ресурсов к сводным задачам.
// Поэтому экспорт таких назначений в формат Primavera может привести к файлам, которые нельзя импортировать в Primavera.
var assignment = project.ResourceAssignments.Add(summaryTask, resource);

var options = new PrimaveraXmlSaveOptions();
options.SkipSummaryAssignments = true;
project.Save(OutDir + "UseSkipSummaryAssignments_out.xml", options);
```

### См. также

* class [PrimaveraSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../primaverasaveoptions/)
* assembly [Aspose.Tasks](../../../)


