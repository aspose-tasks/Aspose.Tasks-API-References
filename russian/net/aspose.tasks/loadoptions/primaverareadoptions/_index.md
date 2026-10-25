---
title: "LoadOptions.PrimaveraReadOptions"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "LoadOptions свойство. Получает или задает указанный экземпляр класса PrimaveraReadOptions, который может использоваться для настройки поведения загрузки форматов Primavera Primavera P6 XER или Primavera P6 Xml"
type: docs
weight: 60
url: /ru/net/aspose.tasks/loadoptions/primaverareadoptions/
---
## LoadOptions.PrimaveraReadOptions property

Получает или задает указанный экземпляр класса [`PrimaveraReadOptions`](../../primaverareadoptions/), который может использоваться для настройки поведения загрузки форматов Primavera (Primavera P6 XER или Primavera P6 Xml).

```csharp
public PrimaveraReadOptions PrimaveraReadOptions { get; set; }
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

* class [PrimaveraReadOptions](../../primaverareadoptions/)
* class [LoadOptions](../)
* namespace [Aspose.Tasks](../../loadoptions/)
* assembly [Aspose.Tasks](../../../)


