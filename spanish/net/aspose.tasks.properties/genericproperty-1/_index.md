---
title: "Estructura GenericPropertyTKey"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Estructura Aspose.Tasks.Properties.GenericProperty1TKey. Representa una propiedad contenedora"
type: docs
weight: 1570
url: /es/net/aspose.tasks.properties/genericproperty-1/
---
## GenericProperty&lt;TKey&gt; structure

Representa una propiedad de contenedor.

```csharp
public struct GenericProperty<TKey>
    where TKey : struct
```

| Parámetro | Descripción |
| --- | --- |
| TKey | El tipo del valor de la propiedad. |

## Constructores

| Nombre | Descripción |
| --- | --- |
| [GenericProperty](genericproperty/)(string) | Inicializa una nueva instancia de la estructura `GenericProperty`. |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [Name](../../aspose.tasks.properties/genericproperty-1/name/) { get; } | Obtiene un nombre de la propiedad. |
| [Value](../../aspose.tasks.properties/genericproperty-1/value/) { get; } | Obtiene un valor de la propiedad. |

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

* namespace [Aspose.Tasks.Properties](../../aspose.tasks.properties/)
* assembly [Aspose.Tasks](../../)


