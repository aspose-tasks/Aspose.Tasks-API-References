---
title: "Rsc.IsBudget"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "Rsc field. يحدد ما إذا كان مورد العمل أو المادة أو التكلفة موردًا ميزانيًا"
type: docs
weight: 380
url: /ar/net/aspose.tasks/rsc/isbudget/
---
## Rsc.IsBudget field

يحدد ما إذا كان مورد العمل أو المادة أو التكلفة هو مورد ميزانية.

```csharp
public static readonly Key<NullableBool, RscKey> IsBudget;
```

## الأمثلة

يعرض كيفية قراءة/كتابة خاصية Rsc.IsBudget.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.IsBudget, true);

Console.WriteLine("Is Budget: " + resource.Get(Rsc.IsBudget));
```

### انظر أيضًا

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


