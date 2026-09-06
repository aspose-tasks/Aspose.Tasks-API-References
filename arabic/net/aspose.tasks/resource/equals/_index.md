---
title: "Resource.Equals"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "طريقة Resource. تُرجع قيمة تشير ما إذا كانت هذه النسخة مساوية لنسخة محددة من فئة Resource."
type: docs
weight: 820
url: /ar/net/aspose.tasks/resource/equals/
---
## Equals(Resource) {#equals}

تُرجع قيمة تشير ما إذا كانت هذه النسخة مساوية لنسخة محددة من الفئة [`Resource`](../).

```csharp
public bool Equals(Resource other)
```

| معامل | النوع | الوصف |
| --- | --- | --- |
| other | Resource | النسخة المحددة من الفئة [`Resource`](../) للمقارنة مع هذه النسخة. |

### قيمة الإرجاع

**True** if the specified instance of the [`Resource`](../) class has the same Uid value as this instance; otherwise, **false**.

## الأمثلة

يوضح كيفية التحقق من مساواة الموارد.

```csharp
var project = new Project(DataDir + "Baselines2010.mpp");

var resource1 = project.Resources.GetById(1);
var resource2 = project.Resources.GetById(1);

Console.WriteLine("Are resources equal: " + resource1.Equals(resource2));
```

### انظر أيضًا

* class [Resource](../)
* namespace [Aspose.Tasks](../../resource/)
* assembly [Aspose.Tasks](../../../)

---

## Equals(object) {#equals_1}

يعيد قيمة تشير إلى ما إذا كانت هذه الحالة مساوية لكائن محدد.

```csharp
public override bool Equals(object obj)
```

| معامل | النوع | الوصف |
| --- | --- | --- |
| obj | كائن | الكائن للمقارنة مع هذه المثيلة. |

### قيمة الإرجاع

**True** if the specified object is a Resource that has the same Uid value as this instance; otherwise, **false**.

## الأمثلة

يوضح كيفية التحقق من مساواة الموارد.

```csharp
var project = new Project(DataDir + "Baselines2010.mpp");

var resource1 = project.Resources.GetById(1);
var resource2 = project.Resources.GetById(1);

Console.WriteLine("Are resources equal: " + resource1.Equals(resource2));
```

### انظر أيضًا

* class [Resource](../)
* namespace [Aspose.Tasks](../../resource/)
* assembly [Aspose.Tasks](../../../)


