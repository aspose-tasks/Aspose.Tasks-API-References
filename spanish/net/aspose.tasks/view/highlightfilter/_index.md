---
title: "View.HighlightFilter"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Propiedad View. Obtiene o establece un valor que indica si Microsoft Project resalta el filtro para una vista única"
type: docs
weight: 40
url: /es/net/aspose.tasks/view/highlightfilter/
---
## View.HighlightFilter property

Obtiene o establece un valor que indica si Microsoft Project resalta el filtro para una vista única.

```csharp
public bool HighlightFilter { get; set; }
```

## Ejemplos

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

* class [View](../)
* namespace [Aspose.Tasks](../../view/)
* assembly [Aspose.Tasks](../../../)


