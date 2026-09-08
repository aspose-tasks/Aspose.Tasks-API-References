---
title: "Clase ViewCollection"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Clase Aspose.Tasks.ViewCollection. Contiene una lista de objetos View. Implementa la interfaz ICollectionView."
type: docs
weight: 2900
url: /es/net/aspose.tasks/viewcollection/
---
## ViewCollection class

Contiene una lista de objetos [`View`](../view/) . Implementa la interfaz ICollection&lt;View&gt;.

```csharp
public class ViewCollection : ICollection<View>
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [Count](../../aspose.tasks/viewcollection/count/) { get; } | Obtiene el número de elementos contenidos en esta colección. |
| [IsReadOnly](../../aspose.tasks/viewcollection/isreadonly/) { get; } | Obtiene un valor que indica si esta colección es de solo lectura; de lo contrario, false. |
| [ParentProject](../../aspose.tasks/viewcollection/parentproject/) { get; } | Obtiene el padre del objeto View. Solo lectura [`Project`](../project/). |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [Add](../../aspose.tasks/viewcollection/add/)(View) | Agrega el elemento especificado a esta colección. |
| [Clear](../../aspose.tasks/viewcollection/clear/)() | Elimina todos los elementos de esta colección. |
| [Contains](../../aspose.tasks/viewcollection/contains/)(View) | Devuelve true si el elemento especificado se encuentra en esta colección; de lo contrario, false. |
| [CopyTo](../../aspose.tasks/viewcollection/copyto/)(View[], int) | Copia los elementos de esta colección al array especificado, comenzando en el índice de array especificado. |
| [GetByName](../../aspose.tasks/viewcollection/getbyname/)(string) | Busca una View con el nombre y devuelve la primera aparición dentro de la colección. |
| [GetByViewScreen](../../aspose.tasks/viewcollection/getbyviewscreen/)(ViewScreen) | Busca una View con la propiedad Screen especificada y devuelve la primera aparición dentro de la colección. |
| [GetEnumerator](../../aspose.tasks/viewcollection/getenumerator/)() | Devuelve un enumerador para esta colección. |
| [Remove](../../aspose.tasks/viewcollection/remove/)(View) | Elimina la primera aparición de un objeto específico de esta colección. |
| [ToList](../../aspose.tasks/viewcollection/tolist/)() | Convierte una colección de vistas en una lista de objetos [`View`](../view/). |

## Ejemplos

Muestra cómo trabajar con colecciones de vistas.

```csharp
var project = new Project(DataDir + "Project1.mpp");

// convertir a una lista simple de vistas
List<View> list = project.Views.ToList();
for (var index = 0; index < list.Count; index++)
{
    var viewToChange = list[index];
    viewToChange.PageInfo.Header.CenteredText = "Header " + index;
}

// agregar una nueva vista
var view = new GanttChartView();
if (!project.Views.IsReadOnly)
{
    project.Views.Add(view);
}

// iterar sobre vistas
Console.WriteLine("Iterate over views of " + project.Views.ParentProject.Get(Prj.Name) + " project.");
Console.WriteLine("Project view count: " + project.Views.Count);
Console.WriteLine();
foreach (var projectView in project.Views)
{
    Console.WriteLine("Name: " + projectView.Name);
}

// eliminar todas las vistas de una vez
project.Views.Clear();

// o una por una
{
    // enfoque 1
    List<View> listToDelete = project.Views.ToList();
    foreach (var v in listToDelete)
    {
        if (project.Views.Contains(v))
        {
            project.Views.Remove(v);
        }
    }
}

{
    // enfoque 2
    var array = new View[project.Views.Count];
    project.Views.CopyTo(array, 0);
    foreach (var v in array)
    {
        if (project.Views.Contains(v))
        {
            project.Views.Remove(v);
        }
    }
}
```

### Ver también

* class [View](../view/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


