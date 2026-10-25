---
title: "Clase View"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Clase Aspose.Tasks.View. Representa una vista en Project"
type: docs
weight: 2890
url: /es/net/aspose.tasks/view/
---
## View class

Representa una vista en Project.

```csharp
public class View : IComparable<View>
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [View](view/#constructor)() | Inicializa una nueva instancia de la clase `View`. |
| [View](view/#constructor_1)(ViewScreen) | Inicializa una nueva instancia de la clase `View`. |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [Filter](../../aspose.tasks/view/filter/) { get; set; } | Obtiene o establece un filtro utilizado en una vista única. |
| [Group](../../aspose.tasks/view/group/) { get; set; } | Obtiene o establece un grupo de la vista única. |
| [HighlightFilter](../../aspose.tasks/view/highlightfilter/) { get; set; } | Obtiene o establece un valor que indica si Microsoft Project resalta el filtro para una vista única. |
| [Name](../../aspose.tasks/view/name/) { get; set; } | Obtiene o establece el nombre de un objeto View. |
| [PageInfo](../../aspose.tasks/view/pageinfo/) { get; } | Obtiene una instancia de la clase [`PageInfo`](./pageinfo/). Representa los datos de configuración de página que están presentes en el formato de archivo mpp. |
| [ParentProject](../../aspose.tasks/view/parentproject/) { get; } | Obtiene el padre del objeto View. Solo lectura [`Project`](../project/). |
| [Screen](../../aspose.tasks/view/screen/) { get; } | Obtiene el tipo de pantalla para la vista única. Solo lectura [`ViewScreen`](../viewscreen/). |
| [ShowInMenu](../../aspose.tasks/view/showinmenu/) { get; set; } | Obtiene o establece un valor que indica si Microsoft Project muestra el nombre de la vista única en las listas desplegables Vista u Otras Vistas en la cinta de opciones. |
| [Table](../../aspose.tasks/view/table/) { get; set; } | Obtiene o establece una tabla de la vista única. |
| [Type](../../aspose.tasks/view/type/) { get; } | Obtiene el tipo de elemento en la vista única, como tareas o recursos. Solo lectura [`ItemType`](../itemtype/). |
| [Uid](../../aspose.tasks/view/uid/) { get; } | Obtiene el identificador único de una vista. |
| [VisualObjectsPlacements](../../aspose.tasks/view/visualobjectsplacements/) { get; } | Obtiene una colección de objetos que representan la ubicación y apariencia de [`OleObject`](../oleobject/) en la vista. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [CompareTo](../../aspose.tasks/view/compareto/)(View) | Compara la instancia actual con otro objeto del mismo tipo y devuelve un entero que indica si la instancia actual precede, sigue o se encuentra en la misma posición en el orden de clasificación que el otro objeto. |
| override [Equals](../../aspose.tasks/view/equals/)(object) | Devuelve un valor que indica si esta instancia es igual a un objeto especificado. |
| override [GetHashCode](../../aspose.tasks/view/gethashcode/)() | Devuelve un valor de código hash para la instancia de la clase [`Resource`](../resource/). |
| [operator ==](../../aspose.tasks/view/op_equality/) | Devuelve un valor que indica si esta instancia es igual a un objeto especificado. |
| [operator &gt;](../../aspose.tasks/view/op_greaterthan/) | Devuelve un valor que indica si esta instancia es mayor que un objeto especificado. |
| [operator &gt;=](../../aspose.tasks/view/op_greaterthanorequal/) | Devuelve un valor que indica si esta instancia es mayor o igual que un objeto especificado. |
| [operator !=](../../aspose.tasks/view/op_inequality/) | Devuelve un valor que indica si esta instancia no es igual a un objeto especificado. |
| [operator &lt;](../../aspose.tasks/view/op_lessthan/) | Devuelve un valor que indica si esta instancia es menor que un objeto especificado. |
| [operator &lt;=](../../aspose.tasks/view/op_lessthanorequal/) | Devuelve un valor que indica si esta instancia es menor o igual que un objeto especificado. |

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


