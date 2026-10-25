---
title: "PrimaveraReadOptions.PreserveUids"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Proprietà PrimaveraReadOptions. Ottiene o imposta un flag che specifica se gli identificatori univoci originali delle entità devono essere preservati"
type: docs
weight: 20
url: /it/net/aspose.tasks/primaverareadoptions/preserveuids/
---
## PrimaveraReadOptions.PreserveUids property

Ottiene o imposta un flag che specifica se gli identificatori univoci originali delle entità devono essere conservati.

```csharp
public bool PreserveUids { get; set; }
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

* class [PrimaveraReadOptions](../)
* namespace [Aspose.Tasks](../../primaverareadoptions/)
* assembly [Aspose.Tasks](../../../)


