---
title: "PrimaveraSaveOptions.RenumberActivityIds"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Propiedad PrimaveraSaveOptions. Obtiene o establece un valor que indica si es necesario renumerar los IDs de actividad"
type: docs
weight: 50
url: /es/net/aspose.tasks.saving/primaverasaveoptions/renumberactivityids/
---
## PrimaveraSaveOptions.RenumberActivityIds property

Obtiene o establece un valor que indica si es necesario renumerar los IDs de actividad.

```csharp
public bool RenumberActivityIds { get; set; }
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


