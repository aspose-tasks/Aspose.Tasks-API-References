---
title: "Resource.ExtendedAttributes"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Propiedad de Resource. Obtiene los valores de un atributo extendido"
type: docs
weight: 320
url: /es/net/aspose.tasks/resource/extendedattributes/
---
## Resource.ExtendedAttributes property

Obtiene los valores de un atributo extendido.

```csharp
public ExtendedAttributeCollection ExtendedAttributes { get; }
```

## Observaciones

Se requieren dos piezas de datos: un puntero a la tabla de atributos extendidos que se especifica ya sea por el ID único o el ID de campo, y el valor que se especifica ya sea con el valor, o un puntero a la lista de valores.

## Ejemplos

Muestra cómo agregar atributos extendidos de recurso.

```csharp
var project = new Project(DataDir + "ResourceExtendedAttributes.mpp");

// Definir atributo extendido
var definition = project.ExtendedAttributes.GetById((int)ExtendedAttributeTask.Number1);
if (definition == null)
{
    definition = ExtendedAttributeDefinition.CreateResourceDefinition(ExtendedAttributeResource.Number1, "Age");
    project.ExtendedAttributes.Add(definition);
}

// Crear atributo extendido y establecer su valor
var attribute = definition.CreateExtendedAttribute();
attribute.NumericValue = 30.5345m;

// Agregar un nuevo recurso y su atributo extendido
var resource = project.Resources.Add("R1");
resource.ExtendedAttributes.Add(attribute);

project.Save(OutDir + "ResourceExtendedAttributes_out.mpp", SaveFileFormat.Mpp);
```

### Ver también

* class [ExtendedAttributeCollection](../../extendedattributecollection/)
* class [Resource](../)
* namespace [Aspose.Tasks](../../resource/)
* assembly [Aspose.Tasks](../../../)


