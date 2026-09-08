---
title: "Rsc.ActiveDirectoryGuid"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Поле Rsc. Active Directory Guid для ресурса"
type: docs
weight: 20
url: /ru/net/aspose.tasks/rsc/activedirectoryguid/
---
## Rsc.ActiveDirectoryGuid field

GUID Active Directory для ресурса.

```csharp
public static readonly Key<string, RscKey> ActiveDirectoryGuid;
```

## Примеры

Показывает, как читать/записывать свойство Rsc.ActiveDirectoryGuid.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.ActiveDirectoryGuid, "8aede269-c574-4a8b-aa74-32bc877a2aef");

Console.WriteLine("Active Directory Guid: " + resource.Get(Rsc.ActiveDirectoryGuid));
```

### См. также

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


