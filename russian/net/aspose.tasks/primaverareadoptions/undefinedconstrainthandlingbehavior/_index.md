---
title: "PrimaveraReadOptions.UndefinedConstraintHandlingBehavior"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Свойство PrimaveraReadOptions. Указывает поведение, используемое для обработки задач с неопределёнными ограничениями, считанными из формата XER."
type: docs
weight: 50
url: /ru/net/aspose.tasks/primaverareadoptions/undefinedconstrainthandlingbehavior/
---
## PrimaveraReadOptions.UndefinedConstraintHandlingBehavior property

Указывает поведение, используемое для обработки задач с неопределёнными ограничениями, считанных из формата XER.

```csharp
public UndefinedConstraintHandlingBehavior UndefinedConstraintHandlingBehavior { get; set; }
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

* enum [UndefinedConstraintHandlingBehavior](../../undefinedconstrainthandlingbehavior/)
* class [PrimaveraReadOptions](../)
* namespace [Aspose.Tasks](../../primaverareadoptions/)
* assembly [Aspose.Tasks](../../../)


