---
title: "Project.DefaultView"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Propiedad del proyecto. Obtiene o establece la vista predeterminada del proyecto"
type: docs
weight: 360
url: /es/net/aspose.tasks/project/defaultview/
---
## Project.DefaultView property

Obtiene o establece la vista predeterminada del proyecto.

```csharp
public View DefaultView { get; set; }
```

## Ejemplos

Muestra cómo trabajar con la vista predeterminada de un proyecto.

```csharp
var project = new Project(DataDir + "TaskUsageViewWithDetails.mpp");

// Obtener vista predeterminada
UsageView view = (TaskUsageView)project.DefaultView;

// La columna de encabezado de detalles no se mostrará
view.DisplayDetailsHeaderColumn = false;
view.RepeatDetailsHeaderOnAllRows = false;
view.AlignDetailsData = HorizontalStringAlignment.Near;
project.Save(OutDir + "task usage1_out.pdf", SaveFileFormat.Pdf);

// Mostrar columna de encabezado de detalles
view.DisplayDetailsHeaderColumn = true;

// Repetir encabezado de detalles en todas las filas de asignaciones
view.RepeatDetailsHeaderOnAllRows = true;
view.AlignDetailsData = HorizontalStringAlignment.Far;
project.Save(OutDir + "task usage2_out.pdf", SaveFileFormat.Pdf);
```

Muestra cómo trabajar con la vista del proyecto y agregar una columna a la vista predeterminada (que se muestra cuando se abre un archivo MPP en MS Project).

```csharp
// crear un proyecto vacío sin vistas
var project = new Project();
project.Set(Prj.Name, "Test View Project");

// Modificar la vista predeterminada (es una vista de diagrama de Gantt).
// O puedes seleccionar la vista por nombre o mediante la pantalla de vista usando la colección project.View.
var view = (GanttChartView) project.DefaultView;

TableField newColumn = new TableField()
{
    AlignData = HorizontalStringAlignment.Center,
    Title = "My new column",
    Width = 30,
    Field = Field.TaskActualDuration
};

view.Table.TableFields.Add(newColumn);

// La bandera WriteViewData debe usarse para persistir las modificaciones de las propiedades de la vista.
project.Save(OutDir + "ModifyView_output.mpp", new Saving.MPPSaveOptions
{
    WriteViewData = true
});
```

### Ver también

* class [View](../../view/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


