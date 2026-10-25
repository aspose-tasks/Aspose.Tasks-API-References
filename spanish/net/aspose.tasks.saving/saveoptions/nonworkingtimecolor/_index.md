---
title: "SaveOptions.NonWorkingTimeColor"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Propiedad SaveOptions. Obtiene o establece el color del tiempo no laborable"
type: docs
weight: 110
url: /es/net/aspose.tasks.saving/saveoptions/nonworkingtimecolor/
---
## SaveOptions.NonWorkingTimeColor property

Obtiene o establece el color del tiempo no laborable.

```csharp
public Color NonWorkingTimeColor { get; set; }
```

## Ejemplos

Muestra cómo establecer un color personalizado para el tiempo no laborable.

```csharp
var project = new Project(DataDir + "ReadCurrencyProperties.mpp");
SaveOptions options = new PdfSaveOptions { NonWorkingTimeColor = Color.LightGray };
project.Save(OutDir + "ReadCurrencyProperties_out.pdf", options);
```

### Ver también

* class [SaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../saveoptions/)
* assembly [Aspose.Tasks](../../../)


