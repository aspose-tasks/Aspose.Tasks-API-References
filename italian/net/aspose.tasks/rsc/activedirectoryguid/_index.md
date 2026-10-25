---
title: "Rsc.ActiveDirectoryGuid"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Campo Rsc. Il Active Directory Guid per una risorsa"
type: docs
weight: 20
url: /it/net/aspose.tasks/rsc/activedirectoryguid/
---
## Rsc.ActiveDirectoryGuid field

Il GUID di Active Directory per una risorsa.

```csharp
public static readonly Key<string, RscKey> ActiveDirectoryGuid;
```

## Esempi

Mostra come leggere/scrivere la proprietà Rsc.ActiveDirectoryGuid.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.ActiveDirectoryGuid, "8aede269-c574-4a8b-aa74-32bc877a2aef");

Console.WriteLine("Active Directory Guid: " + resource.Get(Rsc.ActiveDirectoryGuid));
```

### Vedi anche

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


