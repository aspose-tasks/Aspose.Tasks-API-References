---
title: "XpsOptions.XpsOptions"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "XpsOptions constructor. Initialiseert een nieuw exemplaar van de XpsOptions-klasse"
type: docs
weight: 10
url: /nl/net/aspose.tasks.saving/xpsoptions/xpsoptions/
---
## XpsOptions constructor

Initialiseert een nieuw exemplaar van de [`XpsOptions`](../) klasse.

```csharp
public XpsOptions()
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


