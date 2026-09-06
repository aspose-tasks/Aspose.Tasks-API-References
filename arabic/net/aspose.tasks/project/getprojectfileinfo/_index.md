---
title: "Project.GetProjectFileInfo"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "طريقة Project. قراءة معلومات ملف المشروع من الملف"
type: docs
weight: 1280
url: /ar/net/aspose.tasks/project/getprojectfileinfo/
---
## GetProjectFileInfo(string) {#getprojectfileinfo_1}

قراءة معلومات ملف المشروع من الملف.

```csharp
public static ProjectFileInfo GetProjectFileInfo(string filename)
```

| معامل | النوع | الوصف |
| --- | --- | --- |
| filename | سلسلة | اسم ملف المشروع. |

### قيمة الإرجاع

معلومات ملف المشروع [`ProjectFileInfo`](../../projectfileinfo/).

## الأمثلة

يعرض كيفية قراءة معلومات ملف المشروع التي تم قرأتها من ملف XML.

```csharp
var info = Project.GetProjectFileInfo(DataDir + "Project.xml");
Console.WriteLine("CanRead: " + info.CanRead);
Console.WriteLine("ProjectApplicationInfo: " + info.ProjectApplicationInfo);
Console.WriteLine("ProjectFileFormat: " + info.ProjectFileFormat);
```

### انظر أيضًا

* class [ProjectFileInfo](../../projectfileinfo/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## GetProjectFileInfo(Stream) {#getprojectfileinfo}

يحصل على معلومات ملف المشروع من الدفق.

```csharp
public static ProjectFileInfo GetProjectFileInfo(Stream stream)
```

| معامل | النوع | الوصف |
| --- | --- | --- |
| دفق | دفق | دفق البيانات. |

### قيمة الإرجاع

معلومات ملف المشروع [`ProjectFileInfo`](../../projectfileinfo/).

## الأمثلة

يظهر كيفية قراءة معلومات ملف المشروع لملف XML يُقرأ من تدفق.

```csharp
using (var stream = new FileStream(DataDir + "Project.xml", FileMode.Open))
{
    var info = Project.GetProjectFileInfo(stream);
    Console.WriteLine("CanRead: " + info.CanRead);
    Console.WriteLine("ProjectApplicationInfo: " + info.ProjectApplicationInfo);
    Console.WriteLine("ProjectFileFormat: " + info.ProjectFileFormat);
}
```

### انظر أيضًا

* class [ProjectFileInfo](../../projectfileinfo/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


