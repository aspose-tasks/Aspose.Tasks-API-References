---
title: "PrimaveraReadOptions.ProjectUid"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Свойство PrimaveraReadOptions. Получает или задает UID проекта для чтения из файла, содержащего несколько проектов."
type: docs
weight: 30
url: /ru/net/aspose.tasks/primaverareadoptions/projectuid/
---
## PrimaveraReadOptions.ProjectUid property

Получает или задает UID проекта для чтения из файла, содержащего несколько проектов.

```csharp
public int ProjectUid { get; set; }
```

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

* class [PrimaveraReadOptions](../)
* namespace [Aspose.Tasks](../../primaverareadoptions/)
* assembly [Aspose.Tasks](../../../)


