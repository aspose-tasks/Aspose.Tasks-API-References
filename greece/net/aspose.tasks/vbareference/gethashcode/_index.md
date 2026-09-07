---
title: "VbaReference.GetHashCode"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Μέθοδος VbaReference. Επιστρέφει μια τιμή κώδικα κατακερματισμού για αυτό το VbaReference"
type: docs
weight: 50
url: /el/net/aspose.tasks/vbareference/gethashcode/
---
## VbaReference.GetHashCode method

Επιστρέφει μια τιμή κώδικα κατακερματισμού για αυτό το [`VbaReference`](../).

```csharp
public override int GetHashCode()
```

### Τιμή Επιστροφής

Επιστρέφει μια τιμή κώδικα κατακερματισμού για αυτό το αντικείμενο.

## Παραδείγματα

Δείχνει πώς να λάβετε έναν κώδικα κατακερματισμού μιας αναφοράς VBA.

```csharp
var project = new Project(DataDir + "VbaProject.mpp");

var reference1 = project.VbaProject.References.ToList()[0];
var reference2 = project.VbaProject.References.ToList()[1];

// Ο κώδικας κατακερματισμού μιας αναφοράς είναι ο κώδικας κατακερματισμού του εσωτερικού GUID της αναφοράς.
Console.WriteLine("VBA reference Hash Code: {0}", reference1.GetHashCode());
Console.WriteLine("VBA reference Hash Code: {0}", reference2.GetHashCode());
```

### Δείτε επίσης

* class [VbaReference](../)
* namespace [Aspose.Tasks](../../vbareference/)
* assembly [Aspose.Tasks](../../../)


