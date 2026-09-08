---
title: "Clase OutlineCodeDefinitionCollection"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Clase Aspose.Tasks.OutlineCodeDefinitionCollection. Representa una colección de objetos OutlineCodeDefinition."
type: docs
weight: 1180
url: /es/net/aspose.tasks/outlinecodedefinitioncollection/
---
## OutlineCodeDefinitionCollection class

Representa una colección de objetos [`OutlineCodeDefinition`](../outlinecodedefinition/).

```csharp
public class OutlineCodeDefinitionCollection : IList<OutlineCodeDefinition>
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [Count](../../aspose.tasks/outlinecodedefinitioncollection/count/) { get; } | Obtiene el número de elementos contenidos en esta colección. |
| [IsReadOnly](../../aspose.tasks/outlinecodedefinitioncollection/isreadonly/) { get; } | Obtiene un valor que indica si esta colección es de solo lectura; de lo contrario, false. |
| [Item](../../aspose.tasks/outlinecodedefinitioncollection/item/) { get; set; } | Devuelve o establece el elemento en el índice especificado. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [Add](../../aspose.tasks/outlinecodedefinitioncollection/add/)(OutlineCodeDefinition) | Agrega el elemento especificado a esta colección. |
| [Clear](../../aspose.tasks/outlinecodedefinitioncollection/clear/)() | Elimina todos los elementos de esta colección. |
| [Contains](../../aspose.tasks/outlinecodedefinitioncollection/contains/)(OutlineCodeDefinition) | Devuelve true si el elemento especificado se encuentra en esta colección; de lo contrario, false. |
| [CopyTo](../../aspose.tasks/outlinecodedefinitioncollection/copyto/)(OutlineCodeDefinition[], int) | Copia los elementos de esta colección al array especificado, comenzando en el índice de array especificado. |
| [GetEnumerator](../../aspose.tasks/outlinecodedefinitioncollection/getenumerator/)() | Devuelve un enumerador para esta colección. |
| [IndexOf](../../aspose.tasks/outlinecodedefinitioncollection/indexof/)(OutlineCodeDefinition) | Determina el índice del elemento especificado en esta colección. |
| [Insert](../../aspose.tasks/outlinecodedefinitioncollection/insert/)(int, OutlineCodeDefinition) | Inserta el elemento especificado en el índice especificado. |
| [Remove](../../aspose.tasks/outlinecodedefinitioncollection/remove/)(OutlineCodeDefinition) | Elimina la primera aparición de un objeto específico de esta colección. |
| [RemoveAt](../../aspose.tasks/outlinecodedefinitioncollection/removeat/)(int) | Elimina un elemento en el índice especificado. |
| [ToList](../../aspose.tasks/outlinecodedefinitioncollection/tolist/)() | Convierte este objeto OutlineCodeDefinitionCollection a una lista de objetos [`OutlineCodeDefinition`](../outlinecodedefinition/). |

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

* class [OutlineCodeDefinition](../outlinecodedefinition/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


