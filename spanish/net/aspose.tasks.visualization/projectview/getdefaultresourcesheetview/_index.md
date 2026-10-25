---
title: "ProjectView.GetDefaultResourceSheetView"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Método ProjectView. Incluye columnas de recurso Uid, nombre, tipo, material, etiqueta, iniciales, grupo, unidades máximas, tarifa estándar, tarifa de horas extra, costo por uso, acumulado, calendario base y código"
type: docs
weight: 40
url: /es/net/aspose.tasks.visualization/projectview/getdefaultresourcesheetview/
---
## ProjectView.GetDefaultResourceSheetView method

Incluye columnas de Uid, nombre de recurso, tipo, etiqueta de material, iniciales, grupo, unidades máximas, tarifa estándar, tarifa de horas extra, costo por uso, acumulado en, calendario base y código de recurso.

```csharp
public static ProjectView GetDefaultResourceSheetView()
```

### Valor devuelto

una vista que contiene una lista de [`ResourceViewColumn`](../../resourceviewcolumn/).

## Ejemplos

Muestra cómo guardar un proyecto con la vista de hoja de recursos.

```csharp
var project = new Project(DataDir + "Project2.mpp");
SaveOptions options = new PdfSaveOptions
{
    Timescale = Timescale.Months,
    View = ProjectView.GetDefaultResourceSheetView()
};

project.Save(OutDir + "WorkWithProjectView_ResourceSheetView_out.pdf", options);
```

### Ver también

* class [ProjectView](../)
* namespace [Aspose.Tasks.Visualization](../../projectview/)
* assembly [Aspose.Tasks](../../../)


