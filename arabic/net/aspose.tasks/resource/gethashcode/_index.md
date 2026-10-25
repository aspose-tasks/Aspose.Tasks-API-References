---
title: "Resource.GetHashCode"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "طريقة Resource. تُرجع قيمة hash code للنسخة من فئة Resource"
type: docs
weight: 840
url: /ar/net/aspose.tasks/resource/gethashcode/
---
## Resource.GetHashCode method

تُرجع قيمة hash code للنسخة من فئة [`Resource`](../).

```csharp
public override int GetHashCode()
```

### قيمة الإرجاع

تُرجع قيمة رمز تجزئة لهذا الكائن.

## الأمثلة

يوضح كيفية الحصول على hash code لمورد.

```csharp
var project = new Project(DataDir + "Project.mpp");

var resource1 = project.Resources.GetById(1);
var resource2 = project.Resources.GetById(2);

// hash code لمورد يساوي UID المورد
Console.WriteLine("Resource UID: {0} Hash Code: {1}", resource1.Get(Rsc.Uid), resource1.GetHashCode());
Console.WriteLine("Resource UID: {0} Hash Code: {1}", resource2.Get(Rsc.Uid), resource2.GetHashCode());
```

### انظر أيضًا

* class [Resource](../)
* namespace [Aspose.Tasks](../../resource/)
* assembly [Aspose.Tasks](../../../)


