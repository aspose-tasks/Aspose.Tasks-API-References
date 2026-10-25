---
title: "VbaModuleAttribute.GetHashCode"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Μέθοδος VbaModuleAttribute. Επιστρέφει μια τιμή κώδικα κατακερματισμού για αυτό το VbaModuleAttribute"
type: docs
weight: 40
url: /el/net/aspose.tasks/vbamoduleattribute/gethashcode/
---
## VbaModuleAttribute.GetHashCode method

Επιστρέφει μια τιμή κώδικα κατακερματισμού για αυτό το [`VbaModuleAttribute`](../).

```csharp
public override int GetHashCode()
```

### Τιμή Επιστροφής

Επιστρέφει μια τιμή κώδικα κατακερματισμού για αυτό το αντικείμενο.

## Παραδείγματα

Δείχνει πώς να λάβετε έναν κώδικα κατακερματισμού μιας ιδιότητας μονάδας VBA.

```csharp
var project = new Project(DataDir + "VbaProject.mpp");
var module = project.VbaProject.Modules.ToList()[0];

var attribute1 = module.Attributes.ToList()[0];
var attribute2 = module.Attributes.ToList()[0];

// εκτύπωση κωδικών κατακερματισμού των ιδιοτήτων μονάδας VBA
Console.WriteLine("Hash codes of VBA module attributes are based on key and value hash codes.");
Console.WriteLine("VBA module attribute 1 Hash Code: {0}", attribute1.GetHashCode());
Console.WriteLine("VBA module attribute 2 Hash Code: {0}", attribute2.GetHashCode());
```

### Δείτε επίσης

* class [VbaModuleAttribute](../)
* namespace [Aspose.Tasks](../../vbamoduleattribute/)
* assembly [Aspose.Tasks](../../../)


