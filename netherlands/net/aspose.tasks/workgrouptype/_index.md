---
title: "Enum WorkGroupType"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Aspose.Tasks.WorkGroupType enum. Specificeert het type van een werkgroep"
type: docs
weight: 3620
url: /nl/net/aspose.tasks/workgrouptype/
---
## WorkGroupType enumeration

Specificeert het type van een werkgroep.

```csharp
public enum WorkGroupType
```

### Waarden

| Naam | Waarde | Beschrijving |
| --- | --- | --- |
| Default | `0` | Geeft het standaard werkgroeptype aan. |
| None | `1` | Geeft het type None voor werkgroep aan. |
| Email | `2` | Geeft het e‑mail werkgroeptype aan. |
| Web | `3` | Geeft het web werkgroeptype aan. |

## Voorbeelden

Toont hoe de werkgroep van een resource in te stellen.

```csharp
var project = new Project();

// ...
var resource = project.Resources.Add("Resource");
resource.Set(Rsc.Workgroup, WorkGroupType.Web);

// ...
```

### Zie ook

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


