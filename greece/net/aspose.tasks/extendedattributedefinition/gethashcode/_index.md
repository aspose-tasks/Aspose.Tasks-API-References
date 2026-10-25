---
title: "ExtendedAttributeDefinition.GetHashCode"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Μέθοδος ExtendedAttributeDefinition. Επιστρέφει έναν κωδικό κατακερματισμού για το στιγμιότυπο της κλάσης ExtendedAttributeDefinition."
type: docs
weight: 330
url: /el/net/aspose.tasks/extendedattributedefinition/gethashcode/
---
## ExtendedAttributeDefinition.GetHashCode method

Επιστρέφει έναν κωδικό κατακερματισμού για το στιγμιότυπο της κλάσης [`ExtendedAttributeDefinition`](../).

```csharp
public override int GetHashCode()
```

### Τιμή Επιστροφής

ένας κωδικός κατακερματισμού για αυτό το αντικείμενο.

## Παραδείγματα

Δείχνει πώς να λάβετε έναν κωδικό κατακερματισμού ενός ορισμού εκτεταμένου χαρακτηριστικού.

```csharp
var project = new Project(DataDir + "MultipleOutlineValues2016.mpp");

var attributeDefinition1 = project.ExtendedAttributes.GetById((int)ExtendedAttributeTask.Start3);
var attributeDefinition2 = project.ExtendedAttributes.GetById((int)ExtendedAttributeTask.Duration2);

// ο κωδικός κατακερματισμού ενός ορισμού εκτεταμένου χαρακτηριστικού είναι ίσος με ένα αναγνωριστικό πεδίου.
Console.WriteLine("Extended Attribute Field Id: {0} Hash Code: {1}", attributeDefinition1.FieldId, attributeDefinition1.GetHashCode());
Console.WriteLine("Extended Attribute Field Id: {0} Hash Code: {1}", attributeDefinition2.FieldId, attributeDefinition2.GetHashCode());
```

### Δείτε επίσης

* class [ExtendedAttributeDefinition](../)
* namespace [Aspose.Tasks](../../extendedattributedefinition/)
* assembly [Aspose.Tasks](../../../)


