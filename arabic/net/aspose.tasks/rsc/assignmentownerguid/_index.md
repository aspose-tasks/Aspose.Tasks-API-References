---
title: "Rsc.AssignmentOwnerGuid"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "حقل Rsc. معرف GUID لمالك التعيين"
type: docs
weight: 110
url: /ar/net/aspose.tasks/rsc/assignmentownerguid/
---
## Rsc.AssignmentOwnerGuid field

معرف GUID لمالك التعيين.

```csharp
public static readonly Key<string, RscKey> AssignmentOwnerGuid;
```

## الأمثلة

يعرض كيفية قراءة/كتابة الخاصية Rsc.AssignmentOwnerGuid.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.AssignmentOwnerGuid, "aad9ac22-9f06-4196-906b-916acebcc1c2");

Console.WriteLine("Assignment Owner Guid: " + resource.Get(Rsc.AssignmentOwnerGuid));
```

### انظر أيضًا

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


