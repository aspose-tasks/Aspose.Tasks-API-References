---
title: "ExtendedAttributeDefinition.GetHashCode"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Metodo ExtendedAttributeDefinition. Restituisce un codice hash per l'istanza della classe ExtendedAttributeDefinition."
type: docs
weight: 330
url: /it/net/aspose.tasks/extendedattributedefinition/gethashcode/
---
## ExtendedAttributeDefinition.GetHashCode method

Restituisce un codice hash per l'istanza della classe [`ExtendedAttributeDefinition`](../).

```csharp
public override int GetHashCode()
```

### Valore di ritorno

un codice hash per questo oggetto.

## Esempi

Mostra come ottenere un codice hash di una definizione di attributo esteso.

```csharp
var project = new Project(DataDir + "MultipleOutlineValues2016.mpp");

var attributeDefinition1 = project.ExtendedAttributes.GetById((int)ExtendedAttributeTask.Start3);
var attributeDefinition2 = project.ExtendedAttributes.GetById((int)ExtendedAttributeTask.Duration2);

// Il codice hash di una definizione di attributo esteso è uguale a un ID di campo.
Console.WriteLine("Extended Attribute Field Id: {0} Hash Code: {1}", attributeDefinition1.FieldId, attributeDefinition1.GetHashCode());
Console.WriteLine("Extended Attribute Field Id: {0} Hash Code: {1}", attributeDefinition2.FieldId, attributeDefinition2.GetHashCode());
```

### Vedi anche

* class [ExtendedAttributeDefinition](../)
* namespace [Aspose.Tasks](../../extendedattributedefinition/)
* assembly [Aspose.Tasks](../../../)


