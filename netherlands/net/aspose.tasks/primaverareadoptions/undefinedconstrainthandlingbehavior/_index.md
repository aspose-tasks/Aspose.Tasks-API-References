---
title: "PrimaveraReadOptions.UndefinedConstraintHandlingBehavior"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "PrimaveraReadOptions eigenschap. Specificeert het gedrag dat wordt gebruikt om taken met ongedefinieerde beperkingen, gelezen uit het XER‑formaat, te verwerken."
type: docs
weight: 50
url: /nl/net/aspose.tasks/primaverareadoptions/undefinedconstrainthandlingbehavior/
---
## PrimaveraReadOptions.UndefinedConstraintHandlingBehavior property

Specificeert het gedrag dat wordt gebruikt om taken met ongedefinieerde beperkingen, gelezen uit XER-indeling, te verwerken.

```csharp
public UndefinedConstraintHandlingBehavior UndefinedConstraintHandlingBehavior { get; set; }
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

* enum [UndefinedConstraintHandlingBehavior](../../undefinedconstrainthandlingbehavior/)
* class [PrimaveraReadOptions](../)
* namespace [Aspose.Tasks](../../primaverareadoptions/)
* assembly [Aspose.Tasks](../../../)


