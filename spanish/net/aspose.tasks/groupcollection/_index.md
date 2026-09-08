---
title: "Clase GroupCollection"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Clase Aspose.Tasks.GroupCollection. Contiene una lista de objetos Group. Implementa la interfaz ICollectionGroup."
type: docs
weight: 780
url: /es/net/aspose.tasks/groupcollection/
---
## GroupCollection class

Contiene una lista de objetos [`Group`](../group/). Implementa la interfaz ICollection&lt;Group&gt;.

```csharp
public class GroupCollection : ICollection<Group>
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [Count](../../aspose.tasks/groupcollection/count/) { get; } | Obtiene el número de elementos contenidos en esta colección. |
| [IsReadOnly](../../aspose.tasks/groupcollection/isreadonly/) { get; } | Obtiene un valor que indica si esta colección es de solo lectura. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [Add](../../aspose.tasks/groupcollection/add/)(Group) | Agrega el elemento especificado a esta colección. |
| [Clear](../../aspose.tasks/groupcollection/clear/)() | Elimina todos los elementos de esta colección. |
| [Contains](../../aspose.tasks/groupcollection/contains/)(Group) | Devuelve true si el elemento especificado se encuentra en esta colección; de lo contrario, false. |
| [CopyTo](../../aspose.tasks/groupcollection/copyto/)(Group[], int) | Copia los elementos de esta colección al array especificado, comenzando en el índice de array especificado. |
| [GetEnumerator](../../aspose.tasks/groupcollection/getenumerator/)() | Devuelve un enumerador para esta colección. |
| [Remove](../../aspose.tasks/groupcollection/remove/)(Group) | Elimina la primera aparición de un objeto específico de esta colección. |
| [ToList](../../aspose.tasks/groupcollection/tolist/)() | Convierte una colección de grupos en una lista de objetos [`Group`](../group/). |

## Ejemplos

Muestra cómo trabajar con una colección de grupos.

```csharp
var project = new Project(DataDir + "ReadGroupDefinitionData.mpp");

// iterar sobre grupos de tareas
Console.WriteLine("Print task groups of {0} project: ", project.Get(Prj.Name));
Console.WriteLine("Task Group Count: " + project.TaskGroups.Count);
foreach (var group in project.TaskGroups)
{
    Console.WriteLine("Name: " + group.Name);
    Console.WriteLine("Show In Menu: " + group.ShowInMenu);
    Console.WriteLine();
}

// iterar sobre grupos de recursos
Console.WriteLine("Project resource group count: " + project.ResourceGroups.Count);
foreach (var group in project.ResourceGroups)
{
    Console.WriteLine("Resource group Name: " + group.Name);
    Console.WriteLine("Resource group ShowInMenu" + group.ShowInMenu);
}

var otherProject = new Project(DataDir + "Blank2010.mpp");

// limpiar los grupos del otro proyecto
otherProject.TaskGroups.Clear();

// copiar grupos a otro proyecto
var groups = new Group[project.TaskGroups.Count];
project.TaskGroups.CopyTo(groups, 0);

foreach (var group in groups)
{
    otherProject.TaskGroups.Add(group);
}

// agregar grupo de tareas personalizado
var customGroup = new Group
{
    Name = "Custom Group",
    ShowInMenu = true
};

if (!otherProject.TaskGroups.Contains(customGroup))
{
    if (!otherProject.TaskGroups.IsReadOnly)
    {
        otherProject.TaskGroups.Add(customGroup);
    }
}

// eliminar todos los grupos
List<Group> groupsToDelete = otherProject.TaskGroups.ToList();
foreach (var group in groupsToDelete)
{
    otherProject.TaskGroups.Remove(group);
}
```

### Ver también

* class [Group](../group/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


