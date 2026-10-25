---
title: "ExtendedAttributeDefinition.Equals"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Método ExtendedAttributeDefinition. Devuelve una bandera que indica si esta instancia es igual al objeto especificado."
type: docs
weight: 320
url: /es/net/aspose.tasks/extendedattributedefinition/equals/
---
## ExtendedAttributeDefinition.Equals method

Devuelve una bandera que indica si esta instancia es igual al objeto especificado.

```csharp
public override bool Equals(object obj)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| obj | Objeto | el objeto especificado para comparar con esta instancia. |

### Valor devuelto

una bandera que indica si esta instancia es igual al objeto especificado.

## Ejemplos

Muestra cómo comprobar la igualdad de la definición de atributo extendido.

```csharp
var project = new Project(DataDir + "MultipleOutlineValues2016.mpp");

var attributeDefinition1 = project.ExtendedAttributes.GetById((int)ExtendedAttributeTask.Start3);
var attributeDefinition2 = project.ExtendedAttributes.GetById((int)ExtendedAttributeTask.Duration2);

// la igualdad de los calendarios se verifica contra los IDs de campo de la definición de atributo.
Console.WriteLine("ExtendedAttribute 1 Field Id: " + attributeDefinition1.FieldId);
Console.WriteLine("ExtendedAttribute 2 Field Id: " + attributeDefinition2.FieldId);
Console.WriteLine("Are extended attributes equal: " + attributeDefinition1.Equals(attributeDefinition2));
```

### Ver también

* class [ExtendedAttributeDefinition](../)
* namespace [Aspose.Tasks](../../extendedattributedefinition/)
* assembly [Aspose.Tasks](../../../)


