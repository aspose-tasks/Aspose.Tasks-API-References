---
title: "Rsc.ActiveDirectoryGuid"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Rsc-veld. De Active Directory Guid voor een resource"
type: docs
weight: 20
url: /nl/net/aspose.tasks/rsc/activedirectoryguid/
---
## Rsc.ActiveDirectoryGuid field

De Active Directory‑Guid voor een resource.

```csharp
public static readonly Key<string, RscKey> ActiveDirectoryGuid;
```

## Voorbeelden

Toont hoe u de eigenschap Rsc.ActiveDirectoryGuid kunt lezen/schrijven.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.ActiveDirectoryGuid, "8aede269-c574-4a8b-aa74-32bc877a2aef");

Console.WriteLine("Active Directory Guid: " + resource.Get(Rsc.ActiveDirectoryGuid));
```

### Zie ook

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


