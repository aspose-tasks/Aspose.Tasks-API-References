---
title: "ProjectFileInfo.Equals"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "طريقة ProjectFileInfo. تُرجع قيمة تشير إلى ما إذا كانت هذه المثيلة مساوية لكائن محدد"
type: docs
weight: 50
url: /ar/net/aspose.tasks/projectfileinfo/equals/
---
## Equals(ProjectFileInfo) {#equals}

يعيد قيمة تشير إلى ما إذا كانت هذه الحالة مساوية لكائن محدد.

```csharp
public bool Equals(ProjectFileInfo other)
```

| معامل | النوع | الوصف |
| --- | --- | --- |
| آخر | ProjectFileInfo | الكائن المحدد للمقارنة مع هذه المثيلة. |

### قيمة الإرجاع

تُرجع true إذا كان الـ ProjectFileInfo المحدد وهذه المثيلة لهما تنسيق ملف ومعلومات تطبيق متساوية.

## الأمثلة

يوضح كيفية قراءة معلومات ملف المشروع.

```csharp
var info = Project.GetProjectFileInfo(DataDir + "Project.xml");
Console.WriteLine("CanRead: " + info.CanRead);
Console.WriteLine("ProjectApplicationInfo: " + info.ProjectApplicationInfo);
Console.WriteLine("ProjectFileFormat: " + info.ProjectFileFormat);
```

### انظر أيضًا

* class [ProjectFileInfo](../)
* namespace [Aspose.Tasks](../../projectfileinfo/)
* assembly [Aspose.Tasks](../../../)

---

## Equals(object) {#equals_1}

يعيد قيمة تشير إلى ما إذا كانت هذه الحالة مساوية لكائن محدد.

```csharp
public override bool Equals(object obj)
```

| معامل | النوع | الوصف |
| --- | --- | --- |
| obj | كائن | الكائن المحدد للمقارنة مع هذه المثيلة. |

### قيمة الإرجاع

تُرجع true إذا كان الـ ProjectFileInfo المحدد وهذه المثيلة لهما تنسيق ملف ومعلومات تطبيق متساوية.

## الأمثلة

يوضح كيفية قراءة معلومات ملف المشروع.

```csharp
var info = Project.GetProjectFileInfo(DataDir + "Project.xml");
Console.WriteLine("CanRead: " + info.CanRead);
Console.WriteLine("ProjectApplicationInfo: " + info.ProjectApplicationInfo);
Console.WriteLine("ProjectFileFormat: " + info.ProjectFileFormat);
```

### انظر أيضًا

* class [ProjectFileInfo](../)
* namespace [Aspose.Tasks](../../projectfileinfo/)
* assembly [Aspose.Tasks](../../../)


