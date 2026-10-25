---
title: "Класс PrimaveraSaveOptions"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Класс Aspose.Tasks.Saving.PrimaveraSaveOptions. Позволяет задавать дополнительные параметры при сохранении проекта в формат Primavera XER."
type: docs
weight: 2150
url: /ru/net/aspose.tasks.saving/primaverasaveoptions/
---
## PrimaveraSaveOptions class

Позволяет указать дополнительные параметры при сохранении проекта в формат Primavera XER.

```csharp
public class PrimaveraSaveOptions : SimpleSaveOptions
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [PrimaveraSaveOptions](primaverasaveoptions/)() | Инициализирует новый экземпляр класса `PrimaveraSaveOptions`. |

## Свойства

| Имя | Описание |
| --- | --- |
| [ActivityIdIncrement](../../aspose.tasks.saving/primaverasaveoptions/activityidincrement/) { get; set; } | Получает или задает приращение, используемое при перенумерации идентификаторов задач. |
| [ActivityIdPrefix](../../aspose.tasks.saving/primaverasaveoptions/activityidprefix/) { get; set; } | Получает или задает префикс, используемый при перенумерации идентификаторов задач. |
| [ActivityIdSuffix](../../aspose.tasks.saving/primaverasaveoptions/activityidsuffix/) { get; set; } | Получает или задает суффикс, используемый при перенумерации идентификаторов задач. |
| [RenumberActivityIds](../../aspose.tasks.saving/primaverasaveoptions/renumberactivityids/) { get; set; } | Получает или задает значение, указывающее, необходимо ли перенумеровывать идентификаторы задач. |
| [SaveFormat](../../aspose.tasks.saving/simplesaveoptions/saveformat/) { get; } | Получает или задает формат, в котором будет сохраняться документ, если используется этот объект параметров сохранения. |
| [SkipSummaryAssignments](../../aspose.tasks.saving/primaverasaveoptions/skipsummaryassignments/) { get; set; } | Получает или задаёт значение, указывающее, следует ли пропускать назначения ресурсов к сводным задачам при экспорте. |
| [TasksComparer](../../aspose.tasks.saving/simplesaveoptions/taskscomparer/) { get; set; } | Получает или задает компаратор для сортировки задач на диаграмме Ганта и листе задач. |
| [TasksFilter](../../aspose.tasks.saving/simplesaveoptions/tasksfilter/) { get; set; } | Получает или задает условие, используемое для фильтрации задач, отрисованных на диаграммах Ганта, листе задач и использовании задач. |

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

* class [SimpleSaveOptions](../simplesaveoptions/)
* namespace [Aspose.Tasks.Saving](../../aspose.tasks.saving/)
* assembly [Aspose.Tasks](../../)


