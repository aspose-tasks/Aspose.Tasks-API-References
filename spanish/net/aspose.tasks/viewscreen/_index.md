---
title: "Enumeración ViewScreen"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Enumeración Aspose.Tasks.ViewScreen. Especifica el tipo de pantalla para una vista"
type: docs
weight: 2910
url: /es/net/aspose.tasks/viewscreen/
---
## ViewScreen enumeration

Especifica el tipo de pantalla para una vista.

```csharp
public enum ViewScreen
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| Calendar | `13` | Vista de Calendario. |
| Gantt | `1` | Vista de Gantt. |
| NetworkDiagram | `2` | Vista de Diagrama de Red. |
| RelationshipDiagram | `3` | Vista de Diagrama de Relaciones. |
| ResourceForm | `6` | Vista de Formulario de Recurso. |
| ResourceGraph | `8` | Vista de Gráfico de Recurso. |
| ResourceNameForm | `12` | Vista de Formulario de Nombre de Recurso. |
| ResourceSheet | `7` | Vista de Hoja de Recurso. |
| ResourceUsage | `15` | Vista de Uso de Recurso. |
| TaskDetailsForm | `10` | Vista de Formulario de Detalles de Tarea. |
| TaskForm | `4` | Vista de Formulario de Tarea. |
| TaskNameForm | `11` | Vista de Formulario de Nombre de Tarea. |
| TaskSheet | `5` | Vista de Hoja de Tarea. |
| TaskUsage | `14` | Vista de Uso de Tarea. |

## Ejemplos

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

Muestra cómo trabajar con vistas de MS Project.

```csharp
// crear un proyecto vacío sin vistas
var project = new Project();
project.Set(Prj.Name, "Test View Project");

// crea una vista estándar de diagrama de Gantt
View view = new GanttChartView();

// establece algunas propiedades de la vista
// establece un valor que indica si Microsoft Project muestra el nombre de la vista única en la lista desplegable View u Other Views en la cinta
view.ShowInMenu = true;
// establece un valor que indica si Microsoft Project resalta el filtro para una vista única
view.HighlightFilter = true;

// la escritura de las siguientes propiedades no es compatible
// establece el filtro usado en una vista única
view.Filter = null;
// establece el grupo de la vista única
view.Group = null;
// establece la tabla de la vista única
view.Table = null;

// ajustemos algunas configuraciones de la vista
// establece el número de primeras columnas que se imprimirán en todas las páginas
view.PageInfo.PageViewSettings.FirstColumnsCount = 4;
// establece un valor que indica si se deben imprimir un número especificado de primeras columnas en todas las páginas
view.PageInfo.PageViewSettings.PrintFirstColumnsCountOnAllPages = true;

// agrega la vista a nuestro proyecto
project.Views.Add(view);

// La bandera WriteViewData debe usarse para persistir las modificaciones de project.Views.
project.Save(OutDir + "WorkWithView_output.mpp", new Saving.MPPSaveOptions
{
    WriteViewData = true
});
// verifiquemos algunas propiedades de la vista recién añadida
// imprime el identificador único de una vista
Console.WriteLine("View Uid: " + view.Uid);
// imprime el tipo de pantalla para la vista única
Console.WriteLine("View Screen: " + view.Screen);
Console.WriteLine("View Type: " + view.Type);
Console.WriteLine("Parent Project of the view: " + view.ParentProject.Get(Prj.Name));
```

### Ver también

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


