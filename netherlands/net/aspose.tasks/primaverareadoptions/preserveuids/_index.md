---
title: "PrimaveraReadOptions.PreserveUids"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "PrimaveraReadOptions eigenschap. Haalt of stelt een vlag in die aangeeft of originele unieke identifiers van entiteiten behouden moeten blijven."
type: docs
weight: 20
url: /nl/net/aspose.tasks/primaverareadoptions/preserveuids/
---
## PrimaveraReadOptions.PreserveUids property

Haalt of stelt een vlag in die aangeeft of originele unieke identifiers van entiteiten behouden moeten blijven.

```csharp
public bool PreserveUids { get; set; }
```

## Voorbeelden

Toont hoe een Primavera‑project te laden met de opgegeven Id met behulp van &lt;see cref="LoadOptions" /&gt;.

```csharp
var loadOptions = new LoadOptions();

var primaveraOptions = new PrimaveraReadOptions()
{
    ProjectUid = 3882,
    UndefinedConstraintHandlingBehavior = UndefinedConstraintHandlingBehavior.None,
    PreserveUids = true
};

// stel Primavera leesopties in
loadOptions.PrimaveraReadOptions = primaveraOptions;

var project = new Project(DataDir + "PrimaveraProject.xml", loadOptions);
Console.WriteLine("Project Name: " + project.Get(Prj.Name));

// werken met het project...
```

### Zie ook

* class [PrimaveraReadOptions](../)
* namespace [Aspose.Tasks](../../primaverareadoptions/)
* assembly [Aspose.Tasks](../../../)


