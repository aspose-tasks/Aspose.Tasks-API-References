---
title: "PrimaveraSaveOptions.ActivityIdPrefix"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Propiedad PrimaveraSaveOptions. Obtiene o establece el prefijo usado al renumerar los IDs de actividad"
type: docs
weight: 30
url: /es/net/aspose.tasks.saving/primaverasaveoptions/activityidprefix/
---
## PrimaveraSaveOptions.ActivityIdPrefix property

Obtiene o establece el prefijo utilizado al renumerar los IDs de actividad.

```csharp
public string ActivityIdPrefix { get; set; }
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


