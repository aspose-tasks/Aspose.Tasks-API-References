---
title: "Rsc.ActiveDirectoryGuid"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Rsc field. Guid Active Directory untuk sebuah sumber daya"
type: docs
weight: 20
url: /id/net/aspose.tasks/rsc/activedirectoryguid/
---
## Rsc.ActiveDirectoryGuid field

Guid Active Directory untuk sebuah sumber daya.

```csharp
public static readonly Key<string, RscKey> ActiveDirectoryGuid;
```

## Contoh

Menampilkan cara membaca/menulis properti Rsc.ActiveDirectoryGuid.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.ActiveDirectoryGuid, "8aede269-c574-4a8b-aa74-32bc877a2aef");

Console.WriteLine("Active Directory Guid: " + resource.Get(Rsc.ActiveDirectoryGuid));
```

### Lihat Juga

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


