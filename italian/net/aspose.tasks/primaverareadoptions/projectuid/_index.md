---
title: "PrimaveraReadOptions.ProjectUid"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Proprietà PrimaveraReadOptions. Ottiene o imposta l'UID di un progetto da leggere da un file contenente più progetti"
type: docs
weight: 30
url: /it/net/aspose.tasks/primaverareadoptions/projectuid/
---
## PrimaveraReadOptions.ProjectUid property

Ottiene o imposta l'UID di un progetto da leggere da un file contenente più progetti.

```csharp
public int ProjectUid { get; set; }
```

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

* class [PrimaveraReadOptions](../)
* namespace [Aspose.Tasks](../../primaverareadoptions/)
* assembly [Aspose.Tasks](../../../)


