---
title: "Rsc.IsTeamAssignmentPool"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "حقل Rsc. يوضح ما إذا كان المورد الحالي موردًا فريقًا"
type: docs
weight: 430
url: /ar/net/aspose.tasks/rsc/isteamassignmentpool/
---
## Rsc.IsTeamAssignmentPool field

يعرض ما إذا كان المورد الحالي مورد فريق.

```csharp
public static readonly Key<bool, RscKey> IsTeamAssignmentPool;
```

## الأمثلة

يوضح كيفية قراءة/كتابة خاصية Rsc.IsTeamAssignmentPool.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.IsTeamAssignmentPool, true);

Console.WriteLine("Is Team Assignment Pool: " + resource.Get(Rsc.IsTeamAssignmentPool));
```

### انظر أيضًا

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


