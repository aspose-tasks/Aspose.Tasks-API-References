---
title: "LoadOptions.PrimaveraReadOptions"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "LoadOptions proprietà. Ottiene o imposta un'istanza specificata della classe PrimaveraReadOptions che può essere usata per personalizzare il comportamento del caricamento dei formati Primavera Primavera P6 XER o Primavera P6 Xml"
type: docs
weight: 60
url: /it/net/aspose.tasks/loadoptions/primaverareadoptions/
---
## LoadOptions.PrimaveraReadOptions property

Ottiene o imposta un'istanza specificata della classe [`PrimaveraReadOptions`](../../primaverareadoptions/) che può essere usata per personalizzare il comportamento del caricamento dei formati Primavera (Primavera P6 XER o Primavera P6 Xml).

```csharp
public PrimaveraReadOptions PrimaveraReadOptions { get; set; }
```

## Esempi

Mostra come caricare un progetto Primavera con l'Id specificato utilizzando &lt;see cref="LoadOptions" /&gt;.

```csharp
var loadOptions = new LoadOptions();

var primaveraOptions = new PrimaveraReadOptions()
{
    ProjectUid = 3882,
    UndefinedConstraintHandlingBehavior = UndefinedConstraintHandlingBehavior.None,
    PreserveUids = true
};

// imposta le opzioni di lettura di Primavera
loadOptions.PrimaveraReadOptions = primaveraOptions;

var project = new Project(DataDir + "PrimaveraProject.xml", loadOptions);
Console.WriteLine("Project Name: " + project.Get(Prj.Name));

// lavorare con il progetto...
```

### Vedi anche

* class [PrimaveraReadOptions](../../primaverareadoptions/)
* class [LoadOptions](../)
* namespace [Aspose.Tasks](../../loadoptions/)
* assembly [Aspose.Tasks](../../../)


