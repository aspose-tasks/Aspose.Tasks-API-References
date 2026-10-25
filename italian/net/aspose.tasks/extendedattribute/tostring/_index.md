---
title: "ExtendedAttribute.ToString"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Metodo ExtendedAttribute. Restituisce una breve rappresentazione stringa di un attributo esteso"
type: docs
weight: 110
url: /it/net/aspose.tasks/extendedattribute/tostring/
---
## ExtendedAttribute.ToString method

Restituisce la rappresentazione stringa breve di un attributo esteso.

```csharp
public override string ToString()
```

### Valore di ritorno

La rappresentazione stringa dell'attributo esteso.

## Esempi

Mostra come leggere gli attributi estesi.

```csharp
var project = new Project(DataDir + "ReadTaskExtendedAttributes.mpp");

// Leggi gli attributi estesi per i task
foreach (var task in project.RootTask.Children)
{
    foreach (var attribute in task.ExtendedAttributes)
    {
        // Leggi le informazioni comuni sull'attributo esteso
        Console.WriteLine("Extended Attribute: " + attribute.ToString());
    }
}
```

### Vedi anche

* class [ExtendedAttribute](../)
* namespace [Aspose.Tasks](../../extendedattribute/)
* assembly [Aspose.Tasks](../../../)


