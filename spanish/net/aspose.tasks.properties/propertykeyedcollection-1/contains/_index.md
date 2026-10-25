---
title: "PropertyKeyedCollection1.Contains"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "PropertyKeyedCollection method. Determina si la PropertyCollection contiene una property con el nombre especificado"
type: docs
weight: 60
url: /es/net/aspose.tasks.properties/propertykeyedcollection-1/contains/
---
## PropertyKeyedCollection&lt;T&gt;.Contains method

Determina si la [`PropertyCollection`](../../propertycollection-1/) contiene una property con el nombre especificado.

```csharp
public bool Contains(string name)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| nombre | Cadena | El nombre de una property |

### Valor devuelto

true si la [`PropertyCollection`](../../propertycollection-1/) contiene una property con el nombre especificado; de lo contrario, false.

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

* class [PropertyKeyedCollection&lt;T&gt;](../)
* namespace [Aspose.Tasks.Properties](../../propertykeyedcollection-1/)
* assembly [Aspose.Tasks](../../../)


