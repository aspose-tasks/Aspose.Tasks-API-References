---
title: "GenericProperty1.Name"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Propiedad GenericProperty. Obtiene un nombre de la propiedad"
type: docs
weight: 20
url: /es/net/aspose.tasks.properties/genericproperty-1/name/
---
## GenericProperty&lt;TKey&gt;.Name property

Obtiene un nombre de la propiedad.

```csharp
public string Name { get; }
```

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

* struct [GenericProperty&lt;TKey&gt;](../)
* namespace [Aspose.Tasks.Properties](../../genericproperty-1/)
* assembly [Aspose.Tasks](../../../)


