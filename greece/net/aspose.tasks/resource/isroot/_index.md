---
title: "Resource.IsRoot"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Ιδιότητα Resource. Αποκτά τη σημαία που υποδεικνύει εάν ο πόρος είναι ριζικός πόρος. Ο ριζικός πόρος είναι ένας ειδικός πόρος που προορίζεται για την υποστήριξη των εσωτερικών μορφών MS Projects και δεν προορίζεται να χρησιμοποιείται άμεσα από τον κώδικα των χρηστών"
type: docs
weight: 470
url: /el/net/aspose.tasks/resource/isroot/
---
## Resource.IsRoot property

Λαμβάνει τη σημαία που υποδεικνύει εάν ο πόρος είναι ριζικός πόρος. Ο ριζικός πόρος είναι ένας ειδικός πόρος που προορίζεται να υποστηρίζει τις εσωτερικές λειτουργίες των μορφών του MS Project και δεν προορίζεται να χρησιμοποιείται άμεσα από τον κώδικα του χρήστη.

```csharp
public virtual bool IsRoot { get; }
```

## Παραδείγματα

Δείχνει πώς να χρησιμοποιήσετε την ιδιότητα IsRoot για να παραλείψετε τον ριζικό πόρο.

```csharp
var project = new Project(DataDir + "ResourceCosts.mpp");

foreach (var resource in project.Resources)
{
    if (resource.IsRoot)
    {
        continue;
    }

    Console.WriteLine(resource.Get(Rsc.Name));
}
```

### Δείτε επίσης

* class [Resource](../)
* namespace [Aspose.Tasks](../../resource/)
* assembly [Aspose.Tasks](../../../)


