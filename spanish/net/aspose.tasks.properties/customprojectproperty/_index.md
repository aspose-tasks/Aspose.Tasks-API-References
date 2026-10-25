---
title: "Clase CustomProjectProperty"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Clase Aspose.Tasks.Properties.CustomProjectProperty. Representa una propiedad personalizada"
type: docs
weight: 1540
url: /es/net/aspose.tasks.properties/customprojectproperty/
---
## CustomProjectProperty class

Representa una propiedad personalizada.

```csharp
public sealed class CustomProjectProperty : Property
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [Name](../../aspose.tasks.properties/property/name/) { get; } | Obtiene un nombre de la propiedad. |
| [Type](../../aspose.tasks.properties/customprojectproperty/type/) { get; } | Obtiene un tipo de la propiedad. |
| [Value](../../aspose.tasks.properties/property/value/) { get; set; } | Obtiene o establece un valor de la propiedad. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| override [ToString](../../aspose.tasks.properties/property/tostring/)() | Devuelve el valor de la propiedad como cadena. |

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

* class [Property](../property/)
* namespace [Aspose.Tasks.Properties](../../aspose.tasks.properties/)
* assembly [Aspose.Tasks](../../)


