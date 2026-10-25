---
title: "SaveOptions.NonWorkingTimeColor"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Proprietà SaveOptions. Ottiene o imposta il colore del tempo non lavorativo"
type: docs
weight: 110
url: /it/net/aspose.tasks.saving/saveoptions/nonworkingtimecolor/
---
## SaveOptions.NonWorkingTimeColor property

Ottiene o imposta il colore del tempo non lavorativo.

```csharp
public Color NonWorkingTimeColor { get; set; }
```

## Esempi

Mostra come impostare un colore personalizzato per il tempo non lavorativo.

```csharp
var project = new Project(DataDir + "ReadCurrencyProperties.mpp");
SaveOptions options = new PdfSaveOptions { NonWorkingTimeColor = Color.LightGray };
project.Save(OutDir + "ReadCurrencyProperties_out.pdf", options);
```

### Vedi anche

* class [SaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../saveoptions/)
* assembly [Aspose.Tasks](../../../)


