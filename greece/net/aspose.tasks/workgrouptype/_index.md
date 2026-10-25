---
title: "Enum WorkGroupType"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Aspose.Tasks.WorkGroupType enum. Καθορίζει τον τύπο μιας ομάδας εργασίας"
type: docs
weight: 3620
url: /el/net/aspose.tasks/workgrouptype/
---
## WorkGroupType enumeration

Καθορίζει τον τύπο μιας ομάδας εργασίας.

```csharp
public enum WorkGroupType
```

### Τιμές

| Όνομα | Τιμή | Περιγραφή |
| --- | --- | --- |
| Default | `0` | Δείχνει τον προεπιλεγμένο τύπο ομάδας εργασίας. |
| None | `1` | Δείχνει τον τύπο ομάδας εργασίας 'None'. |
| Email | `2` | Δείχνει τον τύπο ομάδας εργασίας 'Email'. |
| Web | `3` | Δείχνει τον τύπο ομάδας εργασίας 'Web'. |

## Παραδείγματα

Δείχνει πώς να ορίσετε την ομάδα εργασίας ενός πόρου.

```csharp
var project = new Project();

// ...
var resource = project.Resources.Add("Resource");
resource.Set(Rsc.Workgroup, WorkGroupType.Web);

// ...
```

### Δείτε επίσης

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


