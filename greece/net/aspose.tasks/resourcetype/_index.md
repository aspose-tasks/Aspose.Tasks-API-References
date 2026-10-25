---
title: "Απαρίθμηση ResourceType"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Aspose.Tasks.ResourceType enum. Καθορίζει τον τύπο ενός πόρου"
type: docs
weight: 1800
url: /el/net/aspose.tasks/resourcetype/
---
## ResourceType enumeration

Καθορίζει τον τύπο ενός πόρου.

```csharp
public enum ResourceType
```

### Τιμές

| Όνομα | Τιμή | Περιγραφή |
| --- | --- | --- |
| Material | `0` | Δείχνει τον τύπο πόρου Material. |
| Work | `1` | Δείχνει τον τύπο πόρου Work. |
| Cost | `2` | Δείχνει τον τύπο πόρου Cost. |

## Παραδείγματα

Δείχνει πώς να εργαστείτε με τύπους πόρων.

```csharp
var project = new Project();

// προσθέστε έναν πόρο Work
var work = project.Resources.Add("Work resource");
work.Set(Rsc.Type, ResourceType.Work);

// προσθέστε έναν πόρο Material
var material = project.Resources.Add("Material resource");
material.Set(Rsc.Type, ResourceType.Material);
material.Set(Rsc.MaterialLabel, "kg");

// προσθέστε έναν πόρο Material
var cost = project.Resources.Add("Cost resource");
cost.Set(Rsc.Type, ResourceType.Cost);
cost.Set(Rsc.Cost, 59.99m);

// εργαστείτε με πόρους: δημιουργήστε εργασίες, εκχωρήστε πόρους κ.λπ...
```

### Δείτε επίσης

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


