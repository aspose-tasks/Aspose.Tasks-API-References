---
title: "Prj.MicrosoftProjectServerURL"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "حقل Prj. يحدد ما إذا كان المشروع قد تم إنشاؤه بواسطة مستخدم Project Server مقابل مستخدم NT"
type: docs
weight: 460
url: /ar/net/aspose.tasks/prj/microsoftprojectserverurl/
---
## Prj.MicrosoftProjectServerURL field

يحدد ما إذا كان المشروع قد تم إنشاؤه بواسطة مستخدم Project Server بدلاً من مستخدم NT.

```csharp
public static readonly Key<NullableBool, PrjKey> MicrosoftProjectServerURL;
```

## الأمثلة

يوضح كيفية قراءة/كتابة خاصية Prj.MicrosoftProjectServerURL.

```csharp
var project = new Project();

project.Set(Prj.MicrosoftProjectServerURL, true);

Console.WriteLine("Microsoft Project Server U R L: " + project.Get(Prj.MicrosoftProjectServerURL));
```

### انظر أيضًا

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


