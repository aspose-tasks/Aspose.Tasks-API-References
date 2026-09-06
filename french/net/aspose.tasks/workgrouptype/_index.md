---
title: "Enum WorkGroupType"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Aspose.Tasks.WorkGroupType enum. Spécifie le type d'un groupe de travail"
type: docs
weight: 3620
url: /fr/net/aspose.tasks/workgrouptype/
---
## WorkGroupType enumeration

Spécifie le type d'un groupe de travail.

```csharp
public enum WorkGroupType
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| Default | `0` | Indique le type de groupe de travail par défaut. |
| None | `1` | Indique le type de groupe de travail Aucun. |
| Email | `2` | Indique le type de groupe de travail Email. |
| Web | `3` | Indique le type de groupe de travail Web. |

## Exemples

Montre comment définir le groupe de travail d'une ressource.

```csharp
var project = new Project();

// ...
var resource = project.Resources.Add("Resource");
resource.Set(Rsc.Workgroup, WorkGroupType.Web);

// ...
```

### Voir aussi

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


