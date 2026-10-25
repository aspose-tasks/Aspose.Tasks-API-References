---
title: "PrimaveraReadOptions.UndefinedConstraintHandlingBehavior"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Proprietà PrimaveraReadOptions. Specifica il comportamento utilizzato per elaborare le attività con vincoli non definiti letti dal formato XER"
type: docs
weight: 50
url: /it/net/aspose.tasks/primaverareadoptions/undefinedconstrainthandlingbehavior/
---
## PrimaveraReadOptions.UndefinedConstraintHandlingBehavior property

Specifica il comportamento utilizzato per elaborare le attività con vincoli non definiti letti dal formato XER.

```csharp
public UndefinedConstraintHandlingBehavior UndefinedConstraintHandlingBehavior { get; set; }
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

* enum [UndefinedConstraintHandlingBehavior](../../undefinedconstrainthandlingbehavior/)
* class [PrimaveraReadOptions](../)
* namespace [Aspose.Tasks](../../primaverareadoptions/)
* assembly [Aspose.Tasks](../../../)


