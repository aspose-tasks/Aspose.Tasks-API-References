---
title: "XpsOptions.RenderMetafileAsBitmap"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "XpsOptions‑eigenschap. Haalt een waarde op of stelt deze in die aangeeft of een metafile als bitmap moet worden gerenderd."
type: docs
weight: 20
url: /nl/net/aspose.tasks.saving/xpsoptions/rendermetafileasbitmap/
---
## XpsOptions.RenderMetafileAsBitmap property

Haalt op of stelt een waarde in die aangeeft of een metafile als bitmap moet worden gerenderd.

```csharp
public bool RenderMetafileAsBitmap { get; set; }
```

## Voorbeelden

Toont hoe een project kan worden opgeslagen als XPS‑bestand.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

// maak XPS‑opslagopties en stem de parameters af
var options = new XpsOptions
{
    RenderMetafileAsBitmap = true
};

project.Save(OutDir + "UseSvgOptions_out.xps", options);
```

### Zie ook

* class [XpsOptions](../)
* namespace [Aspose.Tasks.Saving](../../xpsoptions/)
* assembly [Aspose.Tasks](../../../)


