---
title: ExtendedAttributeDefinition.CreateLookupResourceDefinition
second_title: Referencia de Aspose.Tasks para la API de .NET
description: ExtendedAttributeDefinition método. Método de fábrica que crea una definición de atributo extendida con búsqueda. TieneCalculationType igual aLookup y solo se puede usar en Recursos. Debe especificarfieldId yalias cuando llame a este método. El tipo de campo se deduce del campo id.
type: docs
weight: 10
url: /es/net/aspose.tasks/extendedattributedefinition/createlookupresourcedefinition/
---
## CreateLookupResourceDefinition(ExtendedAttributeResource, string) {#createlookupresourcedefinition_1}

Método de fábrica que crea una definición de atributo extendida con búsqueda. Tiene[`CalculationType`](../calculationtype/) igual aLookup y solo se puede usar en Recursos. Debe especificar*fieldId* y*alias* cuando llame a este método. El tipo de campo se deduce del campo id.

```csharp
public static ExtendedAttributeDefinition CreateLookupResourceDefinition(
    ExtendedAttributeResource fieldId, string alias)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| fieldId | ExtendedAttributeResource | El especificado[`ExtendedAttributeResource`](../../extendedattributeresource/) identificación de campo |
| alias | String | El especificadoString alias. |

### Valor_devuelto

Instancia creada del[`ExtendedAttributeDefinition`](../) clase con especificado*fieldId* y*alias*.

### Ejemplos

Use este ejemplo para crear una definición de campo personalizado para un recurso con búsqueda y luego rellénelo con valores de texto:

```csharp
var resourceTextAttr = ExtendedAttributeDefinition.CreateLookupResourceDefinition(ExtendedAttributeResource.Text27, "My custom field");
resourceTextAttr.AddLookupValue(new Value { Id = 1, Val = "Text value 1", Description = "Text value description 1" });
resourceTextAttr.AddLookupValue(new Value { Id = 2, Val = "Text value 2", Description = "Text value description 2" });
project.ExtendedAttributes.Add(resourceTextAttr);
```

### Ver también

* enum [ExtendedAttributeResource](../../extendedattributeresource/)
* class [ExtendedAttributeDefinition](../)
* espacio de nombres [Aspose.Tasks](../../extendedattributedefinition/)
* asamblea [Aspose.Tasks](../../../)

---

## CreateLookupResourceDefinition(CustomFieldType, ExtendedAttributeResource, string) {#createlookupresourcedefinition}

Método de fábrica que crea una definición de atributo extendida con búsqueda. Tiene[`CalculationType`](../calculationtype/) igual aLookup y solo se puede usar en Recursos. Debe especificar*customFieldType* ,*fieldId* y*alias* cuando llame a este método.

```csharp
public static ExtendedAttributeDefinition CreateLookupResourceDefinition(
    CustomFieldType customFieldType, ExtendedAttributeResource fieldId, string alias)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| customFieldType | CustomFieldType | El especificado[`CustomFieldType`](../../customfieldtype/) tipo. |
| fieldId | ExtendedAttributeResource | El especificado[`ExtendedAttributeResource`](../../extendedattributeresource/) identificación de campo |
| alias | String | El especificadoString alias. |

### Valor_devuelto

Instancia creada del[`ExtendedAttributeDefinition`](../) clase con especificado*customFieldType* ,*fieldId* y*alias*.

### Ejemplos

Use este ejemplo para crear una definición de campo personalizado para un recurso con búsqueda y luego rellénelo con valores de texto:

```csharp
var resourceTextAttr = ExtendedAttributeDefinition.CreateLookupResourceDefinition(CustomFieldType.Text, ExtendedAttributeResource.Text27, "My custom field");
resourceTextAttr.AddLookupValue(new Value { Id = 1, Val = "Text value 1", Description = "Text value description 1" });
resourceTextAttr.AddLookupValue(new Value { Id = 2, Val = "Text value 2", Description = "Text value description 2" });
project.ExtendedAttributes.Add(resourceTextAttr);
```

### Ver también

* enum [CustomFieldType](../../customfieldtype/)
* enum [ExtendedAttributeResource](../../extendedattributeresource/)
* class [ExtendedAttributeDefinition](../)
* espacio de nombres [Aspose.Tasks](../../extendedattributedefinition/)
* asamblea [Aspose.Tasks](../../../)


