---
title: "Enum WorkGroupType"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Aspose.Tasks.WorkGroupType enum. Especifica el tipo de un grupo de trabajo"
type: docs
weight: 3620
url: /es/net/aspose.tasks/workgrouptype/
---
## WorkGroupType enumeration

Especifica el tipo de un grupo de trabajo.

```csharp
public enum WorkGroupType
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| Default | `0` | Indica el tipo de grupo de trabajo predeterminado. |
| None | `1` | Indica el tipo de grupo de trabajo Ninguno. |
| Email | `2` | Indica el tipo de grupo de trabajo Correo electrónico. |
| Web | `3` | Indica el tipo de grupo de trabajo Web. |

## Ejemplos

Muestra cómo establecer el grupo de trabajo de un recurso.

```csharp
var project = new Project();

// ...
var resource = project.Resources.Add("Resource");
resource.Set(Rsc.Workgroup, WorkGroupType.Web);

// ...
```

### Ver también

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


