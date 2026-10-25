---
title: "CustomProjectPropertyCollection.Remove"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "CustomProjectPropertyCollection method. Elimina una property con el nombre especificado de la colección"
type: docs
weight: 50
url: /es/net/aspose.tasks.properties/customprojectpropertycollection/remove/
---
## CustomProjectPropertyCollection.Remove method

Elimina una propiedad con el nombre especificado de la colección.

```csharp
public bool Remove(string name)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| nombre | Cadena | El nombre de la property sin distinción de mayúsculas. |

### Valor devuelto

True si el elemento se encuentra y elimina con éxito; de lo contrario, false.

## Ejemplos

Muestra cómo trabajar con colecciones de propiedades de proyecto personalizadas.

```csharp
var project = new Project(DataDir + "ReadProjectInfo.mpp");

Console.WriteLine("Is custom properties collection read-only?: " + project.CustomProps.IsReadOnly);

// agreguemos nuevas propiedades personalizadas
// la colección admite tipos Boolean, DateTime, Double, String
project.CustomProps.Add("IsEnterprise", true);
project.CustomProps.Add("Project Start Date", new DateTime(2020, 4, 16, 8, 0, 0));
project.CustomProps.Add("Precision", 10d);
project.CustomProps.Add("Custom Name", "MyProject");

// las propiedades personalizadas están disponibles a través de la colección tipada
Console.WriteLine("Count of custom properties: " + project.CustomProps.Count);
foreach (var property in project.CustomProps)
{
    Console.WriteLine(property.Type);
    Console.WriteLine(property.Name);
    Console.WriteLine(property.Value);
    Console.WriteLine();
}

// obtener el valor de una propiedad personalizada
Console.WriteLine("Custom Name: " + project.CustomProps["Custom Name"]);

// iterar sobre los nombres de las propiedades personalizadas
foreach (var propsName in project.CustomProps.Names)
{
    Console.WriteLine("Name: " + propsName);
    Console.WriteLine();
}

// se puede eliminar un valor por clave de cadena
if (project.CustomProps.Contains("Custom Name"))
{
    project.CustomProps.Remove("Custom Name");
}

// o se puede limpiar la colección completamente
project.CustomProps.Clear();
```

### Ver también

* class [CustomProjectPropertyCollection](../)
* namespace [Aspose.Tasks.Properties](../../customprojectpropertycollection/)
* assembly [Aspose.Tasks](../../../)


