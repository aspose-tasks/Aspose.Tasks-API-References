---
title: "XpsOptions.RenderMetafileAsBitmap"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Proprietà XpsOptions. Ottiene o imposta un valore che indica se un metafile deve essere renderizzato come bitmap"
type: docs
weight: 20
url: /it/net/aspose.tasks.saving/xpsoptions/rendermetafileasbitmap/
---
## XpsOptions.RenderMetafileAsBitmap property

Ottiene o imposta un valore che indica se un metafile deve essere renderizzato come bitmap.

```csharp
public bool RenderMetafileAsBitmap { get; set; }
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


