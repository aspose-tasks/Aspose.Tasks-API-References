---
title: "ExtendedAttributeDefinitionCollection.Remove"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "ExtendedAttributeDefinitionCollection método. Elimina la primera aparición de un objeto específico de esta colección"
type: docs
weight: 130
url: /es/net/aspose.tasks/extendedattributedefinitioncollection/remove/
---
## ExtendedAttributeDefinitionCollection.Remove method

Elimina la primera aparición de un objeto específico de esta colección.

```csharp
public bool Remove(ExtendedAttributeDefinition item)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| elemento | ExtendedAttributeDefinition | el objeto especificado para eliminar. |

### Valor devuelto

true si el objeto especificado se eliminó correctamente de esta colección; de lo contrario, false.

## Ejemplos

Muestra cómo usar colecciones de definiciones de atributos extendidos.

```csharp
var project = new Project(DataDir + "ReadTaskExtendedAttributes.mpp");

if (!project.ExtendedAttributes.IsReadOnly)
{
    if (project.ExtendedAttributes.Count > 0)
    {
        // borrar definiciones de atributos extendidos
        project.ExtendedAttributes.Clear();
    }
}

// crear definición de atributo extendido para una tarea
var taskDefinition = ExtendedAttributeDefinition.CreateTaskDefinition(CustomFieldType.Start, ExtendedAttributeTask.Start7, "Start 7");
project.ExtendedAttributes.Add(taskDefinition);

Console.WriteLine("Iterate over extended attributes of " + project.ExtendedAttributes.ParentProject.Get(Prj.Name) + " project: ");
foreach (var attribute in project.ExtendedAttributes)
{
    Console.WriteLine("Attribute Alias: " + attribute.Alias);
    Console.WriteLine("Attribute CfType: " + attribute.CfType);
    Console.WriteLine();
}

Console.WriteLine();

// trabajar con definiciones de atributos extendidos...
var resourceDefinition = ExtendedAttributeDefinition.CreateResourceDefinition(CustomFieldType.Cost, ExtendedAttributeResource.Cost5, "My cost");

if (!project.ExtendedAttributes.Contains(resourceDefinition))
{
    project.ExtendedAttributes.Add(resourceDefinition);
}

// trabajar con definiciones de atributos extendidos...
var resourceDefinition2 = ExtendedAttributeDefinition.CreateResourceDefinition(CustomFieldType.Number, ExtendedAttributeResource.Cost1, "My Cost 2");

if (project.ExtendedAttributes.IndexOf(resourceDefinition2) < 0)
{
    project.ExtendedAttributes.Insert(0, resourceDefinition2);
}

// trabajar con definiciones de atributos extendidos...

// eliminar atributo extendido por índice
project.ExtendedAttributes.RemoveAt(0);

Console.WriteLine("Print project's extended attributes: ");
Console.WriteLine("Count of project's extended attribute definitions: " + project.ExtendedAttributes.Count);

// usar acceso por índice de colección
Console.WriteLine("Attribute 1 Alias: " + project.ExtendedAttributes[0].Alias);
Console.WriteLine("Attribute 1 CfType: " + project.ExtendedAttributes[0].CfType);
Console.WriteLine("Attribute 2 Alias: " + project.ExtendedAttributes[1].Alias);
Console.WriteLine("Attribute 2 CfType: " + project.ExtendedAttributes[1].CfType);

var otherProject = new Project();

// copiar atributos a otro proyecto
var attributes = new ExtendedAttributeDefinition[project.ExtendedAttributes.Count];
project.ExtendedAttributes.CopyTo(attributes, 0);

foreach (var attribute in attributes)
{
    otherProject.ExtendedAttributes.Add(attribute);
}

Console.WriteLine();
Console.WriteLine("Iterate over other project's extended attributes: ");
foreach (var attribute in otherProject.ExtendedAttributes)
{
    Console.WriteLine("Attribute Alias: " + attribute.Alias);
    Console.WriteLine("Attribute CfType: " + attribute.CfType);
    Console.WriteLine();
}

// eliminar todas las definiciones de atributos extendidos
List<ExtendedAttributeDefinition> definitions = project.ExtendedAttributes.ToList();
foreach (var definition in definitions)
{
    project.ExtendedAttributes.Remove(definition);
}
```

### Ver también

* class [ExtendedAttributeDefinition](../../extendedattributedefinition/)
* class [ExtendedAttributeDefinitionCollection](../)
* namespace [Aspose.Tasks](../../extendedattributedefinitioncollection/)
* assembly [Aspose.Tasks](../../../)


