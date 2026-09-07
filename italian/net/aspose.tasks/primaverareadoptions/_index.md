---
title: "Classe PrimaveraReadOptions"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Classe Aspose.Tasks.PrimaveraReadOptions. Consente di specificare opzioni aggiuntive durante la lettura di file Primavera Xml o Primavera Xer."
type: docs
weight: 1370
url: /it/net/aspose.tasks/primaverareadoptions/
---
## PrimaveraReadOptions class

Consente di specificare opzioni aggiuntive durante la lettura di file Primavera Xml o Primavera Xer.

```csharp
public class PrimaveraReadOptions
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [PrimaveraReadOptions](primaverareadoptions/)() | Inizializza una nuova istanza della classe `PrimaveraReadOptions`. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [PreserveUids](../../aspose.tasks/primaverareadoptions/preserveuids/) { get; set; } | Ottiene o imposta un flag che specifica se gli identificatori univoci originali delle entità devono essere conservati. |
| [ProjectUid](../../aspose.tasks/primaverareadoptions/projectuid/) { get; set; } | Ottiene o imposta l'UID di un progetto da leggere da un file contenente più progetti. |
| [ReadBaselineProjects](../../aspose.tasks/primaverareadoptions/readbaselineprojects/) { get; set; } | Ottiene o imposta un flag che specifica se i progetti di baseline devono essere caricati. Il valore predefinito è true. |
| [UndefinedConstraintHandlingBehavior](../../aspose.tasks/primaverareadoptions/undefinedconstrainthandlingbehavior/) { get; set; } | Specifica il comportamento utilizzato per elaborare le attività con vincoli non definiti letti dal formato XER. |

## Esempi

Mostra come leggere un progetto da un file Primavera XML o Primavera XER contenente più progetti.

```csharp
var options = new PrimaveraReadOptions();
options.ProjectUid = 3881;

// Restituisce il progetto con UID speciale
var project = new Project(DataDir + "PrimaveraProject.xml", options);
Console.WriteLine(project.Get(Prj.Name));
```

### Vedi anche

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


