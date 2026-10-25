---
title: "GroupCollection.Remove"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Método GroupCollection. Elimina la primera aparición de un objeto específico de esta colección"
type: docs
weight: 80
url: /es/net/aspose.tasks/groupcollection/remove/
---
## GroupCollection.Remove method

Elimina la primera aparición de un objeto específico de esta colección.

```csharp
public bool Remove(Group item)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| elemento | Group | el objeto especificado para eliminar. |

### Valor devuelto

true si el objeto especificado se eliminó correctamente de esta colección; de lo contrario, false.

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


