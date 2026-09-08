---
title: "ViewCollection.CopyTo"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Método ViewCollection. Copia los elementos de esta colección al arreglo especificado comenzando en el índice de arreglo especificado"
type: docs
weight: 70
url: /es/net/aspose.tasks/viewcollection/copyto/
---
## ViewCollection.CopyTo method

Copia los elementos de esta colección al array especificado, comenzando en el índice de array especificado.

```csharp
public void CopyTo(View[] array, int arrayIndex)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| arreglo | View[] | el arreglo unidimensional especificado al que copiar los elementos |
| arrayIndex | Int32 | el índice basado en cero del arreglo especificado en el que comienza la copia. |

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

* class [View](../../view/)
* class [ViewCollection](../)
* namespace [Aspose.Tasks](../../viewcollection/)
* assembly [Aspose.Tasks](../../../)


