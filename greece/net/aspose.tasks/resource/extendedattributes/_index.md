---
title: "Resource.ExtendedAttributes"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Ιδιότητα Resource. Λαμβάνει τις τιμές ενός εκτεταμένου χαρακτηριστικού"
type: docs
weight: 320
url: /el/net/aspose.tasks/resource/extendedattributes/
---
## Resource.ExtendedAttributes property

Λαμβάνει τις τιμές ενός επεκταμένου χαρακτηριστικού.

```csharp
public ExtendedAttributeCollection ExtendedAttributes { get; }
```

## Παρατηρήσεις

Απαιτούνται δύο κομμάτια δεδομένων - ένας δείκτης πίσω στον πίνακα εκτεταμένων χαρακτηριστικών που καθορίζεται είτε από το μοναδικό ID είτε από το Field ID, και η τιμή που καθορίζεται είτε με την τιμή, είτε με έναν δείκτη πίσω στη λίστα τιμών.

## Παραδείγματα

Δείχνει πώς να προσθέσετε εκτεταμένα χαρακτηριστικά πόρου.

```csharp
var project = new Project(DataDir + "ResourceExtendedAttributes.mpp");

// Ορίστε εκτεταμένο χαρακτηριστικό
var definition = project.ExtendedAttributes.GetById((int)ExtendedAttributeTask.Number1);
if (definition == null)
{
    definition = ExtendedAttributeDefinition.CreateResourceDefinition(ExtendedAttributeResource.Number1, "Age");
    project.ExtendedAttributes.Add(definition);
}

// Δημιουργήστε εκτεταμένο χαρακτηριστικό και ορίστε την τιμή του
var attribute = definition.CreateExtendedAttribute();
attribute.NumericValue = 30.5345m;

// Προσθέστε έναν νέο πόρο και το εκτεταμένο χαρακτηριστικό του   
var resource = project.Resources.Add("R1");
resource.ExtendedAttributes.Add(attribute);

project.Save(OutDir + "ResourceExtendedAttributes_out.mpp", SaveFileFormat.Mpp);
```

### Δείτε επίσης

* class [ExtendedAttributeCollection](../../extendedattributecollection/)
* class [Resource](../)
* namespace [Aspose.Tasks](../../resource/)
* assembly [Aspose.Tasks](../../../)


