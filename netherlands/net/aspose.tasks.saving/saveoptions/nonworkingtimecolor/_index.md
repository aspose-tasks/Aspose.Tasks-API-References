---
title: "SaveOptions.NonWorkingTimeColor"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "SaveOptions eigenschap. Haalt op of stelt de kleur voor niet-werk tijd in."
type: docs
weight: 110
url: /nl/net/aspose.tasks.saving/saveoptions/nonworkingtimecolor/
---
## SaveOptions.NonWorkingTimeColor property

Haalt op of stelt de kleur voor niet-werkelijke tijd in.

```csharp
public Color NonWorkingTimeColor { get; set; }
```

## Voorbeelden

Toont hoe een aangepaste kleur in te stellen voor niet-werk tijd.

```csharp
var project = new Project(DataDir + "ReadCurrencyProperties.mpp");
SaveOptions options = new PdfSaveOptions { NonWorkingTimeColor = Color.LightGray };
project.Save(OutDir + "ReadCurrencyProperties_out.pdf", options);
```

### Zie ook

* class [SaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../saveoptions/)
* assembly [Aspose.Tasks](../../../)


