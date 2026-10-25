---
title: "OutlineCodeDefinitionCollection.Add"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Método OutlineCodeDefinitionCollection. Añade el elemento especificado a esta colección."
type: docs
weight: 40
url: /es/net/aspose.tasks/outlinecodedefinitioncollection/add/
---
## OutlineCodeDefinitionCollection.Add method

Agrega el elemento especificado a esta colección.

```csharp
public void Add(OutlineCodeDefinition item)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| elemento | OutlineCodeDefinition | el elemento especificado para añadir a esta colección. |

## Ejemplos

Muestra cómo trabajar con colecciones de outline code definition.

```csharp
var project = new Project(DataDir + "OutlineCodes.mpp");

Console.WriteLine("Count of outline code definitions: " + project.OutlineCodes.Count);
foreach (var outlineCode in project.OutlineCodes)
{
    Console.WriteLine("Field Name: " + outlineCode.FieldName);
    Console.WriteLine("Alias: " + outlineCode.Alias);
    Console.WriteLine();
}

// agregar una definición de código de esquema personalizada
var outlineCodeDefinition = new OutlineCodeDefinition { FieldId = ((int)ExtendedAttributeTask.OutlineCode3).ToString("D"), Alias = "My Outline Code" };

var outlineCodeDefinition2 = new OutlineCodeDefinition { FieldId = ((int)ExtendedAttributeTask.OutlineCode1).ToString("D"), Alias = "My Outline Code 2" };

if (!project.OutlineCodes.IsReadOnly)
{
    project.OutlineCodes.Add(outlineCodeDefinition);

    // insertar outline code definition en posición
    project.OutlineCodes.Insert(0, outlineCodeDefinition2);
}

// encontrar el índice del outline code definition
var index = project.OutlineCodes.IndexOf(outlineCodeDefinition);

// editar la definición del código de esquema
project.OutlineCodes[index].Alias = "New Alias";

// ...
// trabajar con definiciones de códigos de esquema
// ...

// eliminar la definición del código de esquema
if (project.OutlineCodes.Contains(outlineCodeDefinition))
{
    project.OutlineCodes.Remove(outlineCodeDefinition);
}

// eliminar una definición de código de esquema por índice
project.OutlineCodes.RemoveAt(0);

var otherProject = new Project(DataDir + "Blank2010.mpp");

// eliminar definiciones de códigos de esquema
otherProject.OutlineCodes.Clear();

// copiar definiciones de códigos de esquema
var outlineCodeDefinitions = new OutlineCodeDefinition[project.OutlineCodes.Count];
project.OutlineCodes.CopyTo(outlineCodeDefinitions, 0);

foreach (var definition in outlineCodeDefinitions)
{
    otherProject.OutlineCodes.Add(definition);
}

// ...
// trabajar con definiciones de códigos de esquema
// ...

// eliminar definiciones de códigos de esquema una por una
List<OutlineCodeDefinition> definitions = otherProject.OutlineCodes.ToList();
foreach (var definition in definitions)
{
    otherProject.OutlineCodes.Remove(definition);
}
```

### Ver también

* class [OutlineCodeDefinition](../../outlinecodedefinition/)
* class [OutlineCodeDefinitionCollection](../)
* namespace [Aspose.Tasks](../../outlinecodedefinitioncollection/)
* assembly [Aspose.Tasks](../../../)


