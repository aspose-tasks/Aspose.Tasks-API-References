---
title: "LoadOptions.PrimaveraReadOptions"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "LoadOptions eigenschap. Haalt een opgegeven instantie van de PrimaveraReadOptions-klasse op of stelt deze in, die kan worden gebruikt om het gedrag bij het laden van Primavera-formaten Primavera P6 XER of Primavera P6 Xml aan te passen"
type: docs
weight: 60
url: /nl/net/aspose.tasks/loadoptions/primaverareadoptions/
---
## LoadOptions.PrimaveraReadOptions property

Haalt een opgegeven instantie van de [`PrimaveraReadOptions`](../../primaverareadoptions/) klasse op of stelt deze in, die kan worden gebruikt om het gedrag bij het laden van Primavera-formaten (Primavera P6 XER of Primavera P6 Xml) aan te passen

```csharp
public PrimaveraReadOptions PrimaveraReadOptions { get; set; }
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

* class [PrimaveraReadOptions](../../primaverareadoptions/)
* class [LoadOptions](../)
* namespace [Aspose.Tasks](../../loadoptions/)
* assembly [Aspose.Tasks](../../../)


