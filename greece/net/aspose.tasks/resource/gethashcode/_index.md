---
title: "Resource.GetHashCode"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Μέθοδος Resource. Επιστρέφει μια τιμή κωδικού κατακερματισμού για την παρουσία της κλάσης Resource."
type: docs
weight: 840
url: /el/net/aspose.tasks/resource/gethashcode/
---
## Resource.GetHashCode method

Επιστρέφει μια τιμή κωδικού κατακερματισμού για την παρουσία της κλάσης [`Resource`](../).

```csharp
public override int GetHashCode()
```

### Τιμή Επιστροφής

επιστρέφει μια τιμή κώδικα κατακερματισμού για αυτό το αντικείμενο.

## Παραδείγματα

Δείχνει πώς να λάβετε έναν κωδικό κατακερματισμού ενός πόρου.

```csharp
var project = new Project(DataDir + "Project.mpp");

var resource1 = project.Resources.GetById(1);
var resource2 = project.Resources.GetById(2);

// ο κωδικός κατακερματισμού ενός πόρου είναι ίσος με το UID του πόρου 
Console.WriteLine("Resource UID: {0} Hash Code: {1}", resource1.Get(Rsc.Uid), resource1.GetHashCode());
Console.WriteLine("Resource UID: {0} Hash Code: {1}", resource2.Get(Rsc.Uid), resource2.GetHashCode());
```

### Δείτε επίσης

* class [Resource](../)
* namespace [Aspose.Tasks](../../resource/)
* assembly [Aspose.Tasks](../../../)


