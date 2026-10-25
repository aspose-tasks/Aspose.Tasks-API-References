---
title: "ViewCollection.GetEnumerator"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Método ViewCollection. Devuelve un enumerador para esta colección"
type: docs
weight: 100
url: /es/net/aspose.tasks/viewcollection/getenumerator/
---
## ViewCollection.GetEnumerator method

Devuelve un enumerador para esta colección.

```csharp
public IEnumerator<View> GetEnumerator()
```

### Valor devuelto

un enumerador para esta colección.

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


