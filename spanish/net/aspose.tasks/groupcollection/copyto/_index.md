---
title: "GroupCollection.CopyTo"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Método GroupCollection. Copia los elementos de esta colección al array especificado comenzando en el índice especificado del array"
type: docs
weight: 60
url: /es/net/aspose.tasks/groupcollection/copyto/
---
## GroupCollection.CopyTo method

Copia los elementos de esta colección al array especificado, comenzando en el índice de array especificado.

```csharp
public void CopyTo(Group[] array, int arrayIndex)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| arreglo | Group[] | el arreglo unidimensional especificado al que copiar los elementos |
| arrayIndex | Int32 | el índice basado en cero del arreglo especificado en el que comienza la copia. |

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

* class [Group](../../group/)
* class [GroupCollection](../)
* namespace [Aspose.Tasks](../../groupcollection/)
* assembly [Aspose.Tasks](../../../)


