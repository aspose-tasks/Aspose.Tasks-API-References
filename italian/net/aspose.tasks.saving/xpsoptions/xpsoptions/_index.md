---
title: "XpsOptions.XpsOptions"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Costruttore di XpsOptions. Inizializza una nuova istanza della classe XpsOptions"
type: docs
weight: 10
url: /it/net/aspose.tasks.saving/xpsoptions/xpsoptions/
---
## XpsOptions constructor

Inizializza una nuova istanza della classe [`XpsOptions`](../).

```csharp
public XpsOptions()
```

## Esempi

Mostra come salvare il progetto come file XPS.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

// crea opzioni di salvataggio XPS e regola i parametri
var options = new XpsOptions
{
    RenderMetafileAsBitmap = true
};

project.Save(OutDir + "UseSvgOptions_out.xps", options);
```

### Vedi anche

* class [XpsOptions](../)
* namespace [Aspose.Tasks.Saving](../../xpsoptions/)
* assembly [Aspose.Tasks](../../../)


