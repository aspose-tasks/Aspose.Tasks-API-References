---
title: ExtendedAttributeDefinition.CreateTaskDefinition
second_title: Referencia de Aspose.Tasks para la API de .NET
description: ExtendedAttributeDefinition método. Método de fábrica que crea una definición de atributo extendida simple que Microsoft Project muestra como Ninguno. TieneCalculationType igual aNone y solo se puede usar en Tareas. Debe especificarcustomFieldType fieldId yalias al llamar a este método.
type: docs
weight: 40
url: /es/net/aspose.tasks/extendedattributedefinition/createtaskdefinition/
---
## CreateTaskDefinition(CustomFieldType, ExtendedAttributeTask, string) {#createtaskdefinition}

Método de fábrica que crea una definición de atributo extendida simple, que Microsoft Project muestra como "Ninguno". Tiene[`CalculationType`](../calculationtype/) igual aNone y solo se puede usar en Tareas. Debe especificar*customFieldType* ,*fieldId* y*alias* al llamar a este método.

```csharp
public static ExtendedAttributeDefinition CreateTaskDefinition(CustomFieldType customFieldType, 
    ExtendedAttributeTask fieldId, string alias)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| customFieldType | CustomFieldType | El especificado[`CustomFieldType`](../../customfieldtype/) tipo. |
| fieldId | ExtendedAttributeTask | El especificado[`ExtendedAttributeTask`](../../extendedattributetask/) identificación de campo |
| alias | String | El especificadoString alias. |

### Valor_devuelto

Instancia creada del[`ExtendedAttributeDefinition`](../) clase con especificado*customFieldType* ,*fieldId* y*alias*.

### Ejemplos

Utilice este ejemplo para crear una definición de campo de texto personalizado:

```csharp
var taskTextAttr = ExtendedAttributeDefinition.CreateTaskDefinition(CustomFieldType.Text, ExtendedAttributeTask.Text27, "My custom field");
project.ExtendedAttributes.Add(taskTextAttr);
```

### Ver también

* enum [CustomFieldType](../../customfieldtype/)
* enum [ExtendedAttributeTask](../../extendedattributetask/)
* class [ExtendedAttributeDefinition](../)
* espacio de nombres [Aspose.Tasks](../../extendedattributedefinition/)
* asamblea [Aspose.Tasks](../../../)

---

## CreateTaskDefinition(ExtendedAttributeTask, string) {#createtaskdefinition_1}

Método de fábrica que crea una definición de atributo extendida simple, que Microsoft Project muestra como "Ninguno". Tiene[`CalculationType`](../calculationtype/) igual aNone y solo se puede usar en Tareas. Debe especificar*fieldId* y*alias* al llamar a este método. El tipo de campo se deduce del campo id.

```csharp
public static ExtendedAttributeDefinition CreateTaskDefinition(ExtendedAttributeTask fieldId, 
    string alias)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| fieldId | ExtendedAttributeTask | El especificado[`ExtendedAttributeTask`](../../extendedattributetask/) identificación de campo |
| alias | String | El especificadoString alias. |

### Valor_devuelto

Instancia creada del[`ExtendedAttributeDefinition`](../) clase con especificado*fieldId* y*alias*.

### Ejemplos

Utilice este ejemplo para crear una definición de campo de texto personalizado:

```csharp
var taskTextAttr = ExtendedAttributeDefinition.CreateTaskDefinition(ExtendedAttributeTask.Text27, "My custom field");
project.ExtendedAttributes.Add(taskTextAttr);
```

### Ver también

* enum [ExtendedAttributeTask](../../extendedattributetask/)
* class [ExtendedAttributeDefinition](../)
* espacio de nombres [Aspose.Tasks](../../extendedattributedefinition/)
* asamblea [Aspose.Tasks](../../../)


