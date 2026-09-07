---
title: "ExtendedAttributeDefinition.Equals"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Metodo ExtendedAttributeDefinition. Restituisce un flag che indica se questa istanza è uguale all'oggetto specificato."
type: docs
weight: 320
url: /it/net/aspose.tasks/extendedattributedefinition/equals/
---
## ExtendedAttributeDefinition.Equals method

Restituisce una flag che indica se questa istanza è uguale all'oggetto specificato.

```csharp
public override bool Equals(object obj)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| obj | Oggetto | l'oggetto specificato da confrontare con questa istanza. |

### Valore di ritorno

un flag che indica se questa istanza è uguale all'oggetto specificato.

## Esempi

Mostra come verificare l'uguaglianza della definizione di attributo esteso.

```csharp
var project = new Project(DataDir + "MultipleOutlineValues2016.mpp");

var attributeDefinition1 = project.ExtendedAttributes.GetById((int)ExtendedAttributeTask.Start3);
var attributeDefinition2 = project.ExtendedAttributes.GetById((int)ExtendedAttributeTask.Duration2);

// L'uguaglianza dei calendari è verificata rispetto agli ID dei campi della definizione di attributo.
Console.WriteLine("ExtendedAttribute 1 Field Id: " + attributeDefinition1.FieldId);
Console.WriteLine("ExtendedAttribute 2 Field Id: " + attributeDefinition2.FieldId);
Console.WriteLine("Are extended attributes equal: " + attributeDefinition1.Equals(attributeDefinition2));
```

### Vedi anche

* class [ExtendedAttributeDefinition](../)
* namespace [Aspose.Tasks](../../extendedattributedefinition/)
* assembly [Aspose.Tasks](../../../)


