---
title: "LoadOptions.CancellationToken"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Propiedad LoadOptions. Obtiene o establece un token que puede usarse para cancelar una operación de carga de proyecto."
type: docs
weight: 20
url: /es/net/aspose.tasks/loadoptions/cancellationtoken/
---
## LoadOptions.CancellationToken property

Obtiene o establece un token que puede usarse para cancelar una operación de carga de proyecto.

```csharp
public CancellationToken CancellationToken { get; set; }
```

## Ejemplos

Muestra cómo pasar CancellationToken para cancelar una operación de carga de proyecto de larga duración.

```csharp
var loadOptions = new LoadOptions();

CancellationTokenSource cts = new CancellationTokenSource();
loadOptions.CancellationToken = cts.Token;

// cts puede pasarse a otro hilo donde se puede llamar al método cts.Cancel() para cancelar la operación de carga del proyecto.
// cts.Cancel();
var project = new Project(DataDir + "PrimaveraProject.xml", loadOptions);
```

### Ver también

* class [LoadOptions](../)
* namespace [Aspose.Tasks](../../loadoptions/)
* assembly [Aspose.Tasks](../../../)


