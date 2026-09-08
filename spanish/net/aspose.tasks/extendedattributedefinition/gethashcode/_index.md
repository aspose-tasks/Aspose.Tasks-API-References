---
title: "ExtendedAttributeDefinition.GetHashCode"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Método ExtendedAttributeDefinition. Devuelve un código hash para la instancia de la clase ExtendedAttributeDefinition."
type: docs
weight: 330
url: /es/net/aspose.tasks/extendedattributedefinition/gethashcode/
---
## ExtendedAttributeDefinition.GetHashCode method

Devuelve un código hash para la instancia de la clase [`ExtendedAttributeDefinition`](../).

```csharp
public override int GetHashCode()
```

### Valor devuelto

un código hash para este objeto.

## Ejemplos

Muestra cómo obtener un código hash de una definición de atributo extendido.

```csharp
var project = new Project(DataDir + "MultipleOutlineValues2016.mpp");

var attributeDefinition1 = project.ExtendedAttributes.GetById((int)ExtendedAttributeTask.Start3);
var attributeDefinition2 = project.ExtendedAttributes.GetById((int)ExtendedAttributeTask.Duration2);

// el código hash de una definición de atributo extendido es igual a un ID de campo.
Console.WriteLine("Extended Attribute Field Id: {0} Hash Code: {1}", attributeDefinition1.FieldId, attributeDefinition1.GetHashCode());
Console.WriteLine("Extended Attribute Field Id: {0} Hash Code: {1}", attributeDefinition2.FieldId, attributeDefinition2.GetHashCode());
```

### Ver también

* class [ExtendedAttributeDefinition](../)
* namespace [Aspose.Tasks](../../extendedattributedefinition/)
* assembly [Aspose.Tasks](../../../)


