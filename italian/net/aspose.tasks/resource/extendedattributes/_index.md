---
title: "Resource.ExtendedAttributes"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Proprietà Resource. Ottiene i valori di un attributo esteso"
type: docs
weight: 320
url: /it/net/aspose.tasks/resource/extendedattributes/
---
## Resource.ExtendedAttributes property

Ottiene i valori di un attributo esteso.

```csharp
public ExtendedAttributeCollection ExtendedAttributes { get; }
```

## Osservazioni

Sono necessari due dati - un puntatore alla tabella degli attributi estesi, specificata o dall'ID univoco o dal Field ID, e il valore, specificato o con il valore stesso, o con un puntatore alla lista dei valori.

## Esempi

Mostra come aggiungere attributi estesi della risorsa.

```csharp
var project = new Project(DataDir + "ResourceExtendedAttributes.mpp");

// Definisci attributo esteso
var definition = project.ExtendedAttributes.GetById((int)ExtendedAttributeTask.Number1);
if (definition == null)
{
    definition = ExtendedAttributeDefinition.CreateResourceDefinition(ExtendedAttributeResource.Number1, "Age");
    project.ExtendedAttributes.Add(definition);
}

// Crea attributo esteso e imposta il suo valore
var attribute = definition.CreateExtendedAttribute();
attribute.NumericValue = 30.5345m;

// Aggiungi una nuova risorsa e il suo attributo esteso   
var resource = project.Resources.Add("R1");
resource.ExtendedAttributes.Add(attribute);

project.Save(OutDir + "ResourceExtendedAttributes_out.mpp", SaveFileFormat.Mpp);
```

### Vedi anche

* class [ExtendedAttributeCollection](../../extendedattributecollection/)
* class [Resource](../)
* namespace [Aspose.Tasks](../../resource/)
* assembly [Aspose.Tasks](../../../)


