---
title: "Перечисление WorkGroupType"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Перечисление Aspose.Tasks.WorkGroupType. Указывает тип рабочей группы"
type: docs
weight: 3620
url: /ru/net/aspose.tasks/workgrouptype/
---
## WorkGroupType enumeration

Указывает тип рабочей группы.

```csharp
public enum WorkGroupType
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| Default | `0` | Указывает тип рабочей группы по умолчанию. |
| None | `1` | Указывает тип рабочей группы 'None'. |
| Email | `2` | Указывает тип рабочей группы 'Email'. |
| Web | `3` | Указывает тип рабочей группы 'Web'. |

## Примеры

Показывает, как установить рабочую группу ресурса.

```csharp
var project = new Project();

// ...
var resource = project.Resources.Add("Resource");
resource.Set(Rsc.Workgroup, WorkGroupType.Web);

// ...
```

### См. также

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


