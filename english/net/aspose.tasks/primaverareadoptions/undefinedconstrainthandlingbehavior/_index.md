---
title: PrimaveraReadOptions.UndefinedConstraintHandlingBehavior
second_title: Aspose.Tasks for .NET API Reference
description: PrimaveraReadOptions property. Specifies the behavior used to process tasks with undefined constraints read from XER format
type: docs
weight: 50
url: /net/aspose.tasks/primaverareadoptions/undefinedconstrainthandlingbehavior/
---
## PrimaveraReadOptions.UndefinedConstraintHandlingBehavior property

Specifies the behavior used to process tasks with undefined constraints read from XER format.

```csharp
public UndefinedConstraintHandlingBehavior UndefinedConstraintHandlingBehavior { get; set; }
```

## Examples

Shows how to load Primavera project with the specified Id using &lt;see cref="LoadOptions" /&gt;.

```csharp
var loadOptions = new LoadOptions();

var primaveraOptions = new PrimaveraReadOptions()
{
    ProjectUid = 3882,
    UndefinedConstraintHandlingBehavior = UndefinedConstraintHandlingBehavior.None,
    PreserveUids = true
};

// set Primavera reading options
loadOptions.PrimaveraReadOptions = primaveraOptions;

var project = new Project(DataDir + "PrimaveraProject.xml", loadOptions);
Console.WriteLine("Project Name: " + project.Get(Prj.Name));

// work with the project...
```

### See Also

* enum [UndefinedConstraintHandlingBehavior](../../undefinedconstrainthandlingbehavior/)
* class [PrimaveraReadOptions](../)
* namespace [Aspose.Tasks](../../primaverareadoptions/)
* assembly [Aspose.Tasks](../../../)


