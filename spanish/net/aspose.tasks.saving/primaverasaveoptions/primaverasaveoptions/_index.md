---
title: "PrimaveraSaveOptions.PrimaveraSaveOptions"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Constructor PrimaveraSaveOptions. Inicializa una nueva instancia de la clase PrimaveraSaveOptions"
type: docs
weight: 10
url: /es/net/aspose.tasks.saving/primaverasaveoptions/primaverasaveoptions/
---
## PrimaveraSaveOptions constructor

Inicializa una nueva instancia de la clase [`PrimaveraSaveOptions`](../).

```csharp
public PrimaveraSaveOptions()
```

## Ejemplos

Muestra cómo trabajar con &lt;see cref=\"Aspose.Tasks.Saving.PrimaveraSaveOptions\" /&gt;.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

// crear opciones de guardado Primavera y afinarlas
var options = new PrimaveraSaveOptions
                  {
                      // definir prefijo y sufijo de una actividad
                      ActivityIdPrefix = "TEST",
                      ActivityIdSuffix = 10000,

                      // controlar la renumeración de actividades
                      ActivityIdIncrement = 5,
                      RenumberActivityIds = true
                  };

project.Save(OutDir + "WorkWithPrimaveraSaveOptions_out.xer", options);
```

### Ver también

* class [PrimaveraSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../primaverasaveoptions/)
* assembly [Aspose.Tasks](../../../)


