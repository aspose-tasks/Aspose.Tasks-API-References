---
title: "Rsc.ActiveDirectoryGuid"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "حقل Rsc. معرف Active Directory لمورد"
type: docs
weight: 20
url: /ar/net/aspose.tasks/rsc/activedirectoryguid/
---
## Rsc.ActiveDirectoryGuid field

معرف الـ GUID في Active Directory للمورد.

```csharp
public static readonly Key<string, RscKey> ActiveDirectoryGuid;
```

## الأمثلة

يوضح كيفية قراءة/كتابة خاصية Rsc.ActiveDirectoryGuid.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.ActiveDirectoryGuid, "8aede269-c574-4a8b-aa74-32bc877a2aef");

Console.WriteLine("Active Directory Guid: " + resource.Get(Rsc.ActiveDirectoryGuid));
```

### انظر أيضًا

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


