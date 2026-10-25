---
title: "Класс PrimaveraReadOptions"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Класс Aspose.Tasks.PrimaveraReadOptions. Позволяет задавать дополнительные параметры при чтении файлов Primavera Xml или Primavera Xer."
type: docs
weight: 1370
url: /ru/net/aspose.tasks/primaverareadoptions/
---
## PrimaveraReadOptions class

Позволяет указывать дополнительные параметры при чтении файлов Primavera Xml или Primavera Xer.

```csharp
public class PrimaveraReadOptions
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [PrimaveraReadOptions](primaverareadoptions/)() | Инициализирует новый экземпляр класса `PrimaveraReadOptions`. |

## Свойства

| Имя | Описание |
| --- | --- |
| [PreserveUids](../../aspose.tasks/primaverareadoptions/preserveuids/) { get; set; } | Получает или задает флаг, указывающий, следует ли сохранять оригинальные уникальные идентификаторы сущностей. |
| [ProjectUid](../../aspose.tasks/primaverareadoptions/projectuid/) { get; set; } | Получает или задает UID проекта для чтения из файла, содержащего несколько проектов. |
| [ReadBaselineProjects](../../aspose.tasks/primaverareadoptions/readbaselineprojects/) { get; set; } | Получает или задает флаг, указывающий, следует ли загружать базовые проекты. Значение по умолчанию — true. |
| [UndefinedConstraintHandlingBehavior](../../aspose.tasks/primaverareadoptions/undefinedconstrainthandlingbehavior/) { get; set; } | Указывает поведение, используемое для обработки задач с неопределёнными ограничениями, считанных из формата XER. |

## Примеры

Показывает, как прочитать проект из файла Primavera XML или Primavera XER, содержащего несколько проектов.

```csharp
var options = new PrimaveraReadOptions();
options.ProjectUid = 3881;

// Возвращает проект со специальным UID
var project = new Project(DataDir + "PrimaveraProject.xml", options);
Console.WriteLine(project.Get(Prj.Name));
```

### См. также

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


