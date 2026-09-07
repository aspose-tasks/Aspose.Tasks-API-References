---
title: "Enum WorkGroupType"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Enum Aspose.Tasks.WorkGroupType. Specifica il tipo di gruppo di lavoro"
type: docs
weight: 3620
url: /it/net/aspose.tasks/workgrouptype/
---
## WorkGroupType enumeration

Specifica il tipo di un gruppo di lavoro.

```csharp
public enum WorkGroupType
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| Default | `0` | Indica il tipo di gruppo di lavoro predefinito. |
| None | `1` | Indica il tipo di gruppo di lavoro Nessuno. |
| Email | `2` | Indica il tipo di gruppo di lavoro Email. |
| Web | `3` | Indica il tipo di gruppo di lavoro Web. |

## Esempi

Mostra come impostare il gruppo di lavoro di una risorsa.

```csharp
var project = new Project();

// ...
var resource = project.Resources.Add("Resource");
resource.Set(Rsc.Workgroup, WorkGroupType.Web);

// ...
```

### Vedi anche

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


