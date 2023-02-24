---
title: ExtendedAttributeDefinition.AddLookupValue
second_title: Riferimento all'API di Aspose.Tasks per .NET
description: ExtendedAttributeDefinition metodo. Aggiunge un valore allelenco di ricerca interno. Questo è un modo preferibile per le manipolazioni con ilValueList .
type: docs
weight: 290
url: /it/net/aspose.tasks/extendedattributedefinition/addlookupvalue/
---
## ExtendedAttributeDefinition.AddLookupValue method

Aggiunge un valore all'elenco di ricerca interno. Questo è un modo preferibile per le manipolazioni con il[`ValueList`](../valuelist/) .

```csharp
public void AddLookupValue(Value value)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | Value | Valore da aggiungere alla ricerca. |

### Osservazioni

Questo metodo funziona solo per[`ExtendedAttributeDefinition`](../) instances che hanno[`CalculationType`](../calculationtype/) uguale aLookup .

### Esempi

Usa questo codice per aggiungere un nuovo valore all'elenco di ricerca:

```csharp
taskTextAttr.AddLookupValue(new Value { Id = 1, Val = "Text value 1", Description = "Text value description 1" });
```

### Guarda anche

* class [Value](../../value/)
* class [ExtendedAttributeDefinition](../)
* spazio dei nomi [Aspose.Tasks](../../extendedattributedefinition/)
* assemblea [Aspose.Tasks](../../../)


