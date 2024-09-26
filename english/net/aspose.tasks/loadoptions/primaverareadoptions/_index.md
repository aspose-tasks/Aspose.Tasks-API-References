---
title: LoadOptions.PrimaveraReadOptions
second_title: Aspose.Tasks for .NET API Reference
description: LoadOptions property. Gets or sets a specified instance of the PrimaveraReadOptions class which can be used to customize the behavior of loading Primavera formats Primavera P6 XER or Primavera P6 Xml
type: docs
weight: 60
url: /net/aspose.tasks/loadoptions/primaverareadoptions/
---
## LoadOptions.PrimaveraReadOptions property

Gets or sets a specified instance of the [`PrimaveraReadOptions`](../../primaverareadoptions/) class which can be used to customize the behavior of loading Primavera formats (Primavera P6 XER or Primavera P6 Xml).

```csharp
public PrimaveraReadOptions PrimaveraReadOptions { get; set; }
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

* class [PrimaveraReadOptions](../../primaverareadoptions/)
* class [LoadOptions](../)
* namespace [Aspose.Tasks](../../loadoptions/)
* assembly [Aspose.Tasks](../../../)


