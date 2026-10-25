---
title: "ResourceAssignment.GetHashCode"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Μέθοδος ResourceAssignment. Επιστρέφει μια τιμή hash code για το παράδειγμα της κλάσης ResourceAssignment"
type: docs
weight: 710
url: /el/net/aspose.tasks/resourceassignment/gethashcode/
---
## ResourceAssignment.GetHashCode method

Επιστρέφει μια τιμή hash code για το παράδειγμα της κλάσης [`ResourceAssignment`](../).

```csharp
public override int GetHashCode()
```

### Τιμή Επιστροφής

επιστρέφει μια τιμή κώδικα κατακερματισμού για αυτό το αντικείμενο.

## Παραδείγματα

Δείχνει πώς να λάβετε έναν hash code μιας ανάθεσης πόρων.

```csharp
var project = new Project(DataDir + "BaselineTD2010_3.mpp");

var resourceAssignment1 = project.ResourceAssignments.GetByUid(2);
var resourceAssignment2 = project.ResourceAssignments.GetByUid(3);

// εκτυπώστε τους hash code της ανάθεσης
Console.WriteLine("Resource Assignment 1 Hash Code: {0}", resourceAssignment1.GetHashCode());
Console.WriteLine("Resource Assignment 2 Hash Code: {0}", resourceAssignment2.GetHashCode());
```

### Δείτε επίσης

* class [ResourceAssignment](../)
* namespace [Aspose.Tasks](../../resourceassignment/)
* assembly [Aspose.Tasks](../../../)


