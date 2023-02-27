---
title: ExtendedAttributeDefinition.AddLookupValue
second_title: Referencia de Aspose.Tasks para la API de .NET
description: ExtendedAttributeDefinition método. Agrega un valor a la lista de búsqueda interna. Esta es una forma preferible para las manipulaciones con elValueList .
type: docs
weight: 290
url: /es/net/aspose.tasks/extendedattributedefinition/addlookupvalue/
---
## ExtendedAttributeDefinition.AddLookupValue method

Agrega un valor a la lista de búsqueda interna. Esta es una forma preferible para las manipulaciones con el[`ValueList`](../valuelist/) .

```csharp
public void AddLookupValue(Value value)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| value | Value | Valor para agregar en la búsqueda. |

### Observaciones

Este método solo funciona para[`ExtendedAttributeDefinition`](../) instancias que tienen[`CalculationType`](../calculationtype/) igual aLookup .

### Ejemplos

Use este código para agregar un nuevo valor a la lista de búsqueda:

```csharp
taskTextAttr.AddLookupValue(new Value { Id = 1, Val = "Text value 1", Description = "Text value description 1" });
```

### Ver también

* class [Value](../../value/)
* class [ExtendedAttributeDefinition](../)
* espacio de nombres [Aspose.Tasks](../../extendedattributedefinition/)
* asamblea [Aspose.Tasks](../../../)


