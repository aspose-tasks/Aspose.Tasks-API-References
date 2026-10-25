---
title: "PrimaveraReadOptions.PreserveUids"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Свойство PrimaveraReadOptions. Получает или задает флаг, указывающий, следует ли сохранять оригинальные уникальные идентификаторы сущностей."
type: docs
weight: 20
url: /ru/net/aspose.tasks/primaverareadoptions/preserveuids/
---
## PrimaveraReadOptions.PreserveUids property

Получает или задает флаг, указывающий, следует ли сохранять оригинальные уникальные идентификаторы сущностей.

```csharp
public bool PreserveUids { get; set; }
```

## Примеры

Показывает, как загрузить проект Primavera с указанным Id, используя &lt;see cref=\"LoadOptions\" /&gt;.

```csharp
var loadOptions = new LoadOptions();

var primaveraOptions = new PrimaveraReadOptions()
{
    ProjectUid = 3882,
    UndefinedConstraintHandlingBehavior = UndefinedConstraintHandlingBehavior.None,
    PreserveUids = true
};

// установить параметры чтения Primavera
loadOptions.PrimaveraReadOptions = primaveraOptions;

var project = new Project(DataDir + "PrimaveraProject.xml", loadOptions);
Console.WriteLine("Project Name: " + project.Get(Prj.Name));

// работать с проектом...
```

### См. также

* class [PrimaveraReadOptions](../)
* namespace [Aspose.Tasks](../../primaverareadoptions/)
* assembly [Aspose.Tasks](../../../)


