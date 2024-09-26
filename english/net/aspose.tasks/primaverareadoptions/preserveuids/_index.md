---
title: PrimaveraReadOptions.PreserveUids
second_title: Aspose.Tasks for .NET API Reference
description: PrimaveraReadOptions property. Gets or sets a flag that specifies whether original unique identifiers of entities should be preserved
type: docs
weight: 20
url: /net/aspose.tasks/primaverareadoptions/preserveuids/
---
## PrimaveraReadOptions.PreserveUids property

Gets or sets a flag that specifies whether original unique identifiers of entities should be preserved.

```csharp
public bool PreserveUids { get; set; }
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

* class [PrimaveraReadOptions](../)
* namespace [Aspose.Tasks](../../primaverareadoptions/)
* assembly [Aspose.Tasks](../../../)


