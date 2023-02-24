---
title: ExtendedAttributeDefinition.CreateResourceDefinition
second_title: Referencia de Aspose.Tasks para la API de .NET
description: ExtendedAttributeDefinition método. Método de fábrica que crea una definición de atributo extendida simple que Microsoft Project muestra como Ninguno. TieneCalculationType igual aNone y solo se puede usar en Recurso. Debe especificarcustomFieldType fieldId yalias cuando llame a este método.
type: docs
weight: 30
url: /es/net/aspose.tasks/extendedattributedefinition/createresourcedefinition/
---
## CreateResourceDefinition(CustomFieldType, ExtendedAttributeResource, string) {#createresourcedefinition}

Método de fábrica que crea una definición de atributo extendida simple, que Microsoft Project muestra como "Ninguno". Tiene[`CalculationType`](../calculationtype/) igual aNone y solo se puede usar en Recurso. Debe especificar*customFieldType* ,*fieldId* y*alias* cuando llame a este método.

```csharp
public static ExtendedAttributeDefinition CreateResourceDefinition(CustomFieldType customFieldType, 
    ExtendedAttributeResource fieldId, string alias)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| customFieldType | CustomFieldType | El especificado[`CustomFieldType`](../../customfieldtype/) tipo. |
| fieldId | ExtendedAttributeResource | El especificado[`ExtendedAttributeResource`](../../extendedattributeresource/) identificación de campo |
| alias | String | El especificadoString alias. |

### Valor_devuelto

Instancia creada del[`ExtendedAttributeDefinition`](../) clase con especificado*customFieldType* ,*fieldId* y*alias*.

### Ejemplos

Utilice este ejemplo para crear una definición de campo de texto personalizado:

```csharp
var resourceTextAttr = ExtendedAttributeDefinition.CreateResourceDefinition(CustomFieldType.Text, ExtendedAttributeResource.Text27, "My custom field");
project.ExtendedAttributes.Add(resourceTextAttr);
```

### Ver también

* enum [CustomFieldType](../../customfieldtype/)
* enum [ExtendedAttributeResource](../../extendedattributeresource/)
* class [ExtendedAttributeDefinition](../)
* espacio de nombres [Aspose.Tasks](../../extendedattributedefinition/)
* asamblea [Aspose.Tasks](../../../)

---

## CreateResourceDefinition(ExtendedAttributeResource, string) {#createresourcedefinition_1}

Método de fábrica que crea una definición de atributo extendida simple, que Microsoft Project muestra como "Ninguno". Tiene[`CalculationType`](../calculationtype/) igual aNone y solo se puede usar en Recurso. Debe especificar*fieldId* y*alias* cuando llame a este método. El tipo de campo se deduce del campo id.

```csharp
public static ExtendedAttributeDefinition CreateResourceDefinition(
    ExtendedAttributeResource fieldId, string alias)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| fieldId | ExtendedAttributeResource | El especificado[`ExtendedAttributeResource`](../../extendedattributeresource/) identificación de campo |
| alias | String | El especificadoString alias. |

### Valor_devuelto

Instancia creada del[`ExtendedAttributeDefinition`](../) clase con especificado*fieldId* y*alias*.

### Ejemplos

Utilice este ejemplo para crear una definición de campo de texto personalizado:

```csharp
var resourceTextAttr = ExtendedAttributeDefinition.CreateResourceDefinition(ExtendedAttributeResource.Text27, "My custom field");
project.ExtendedAttributes.Add(resourceTextAttr);
```

### Ver también

* enum [ExtendedAttributeResource](../../extendedattributeresource/)
* class [ExtendedAttributeDefinition](../)
* espacio de nombres [Aspose.Tasks](../../extendedattributedefinition/)
* asamblea [Aspose.Tasks](../../../)


