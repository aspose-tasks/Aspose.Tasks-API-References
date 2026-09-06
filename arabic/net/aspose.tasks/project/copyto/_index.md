---
title: "Project.CopyTo"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "طريقة Project. تنسخ البيانات والخصائص الرئيسية للمشروع إلى مشروع آخر"
type: docs
weight: 1060
url: /ar/net/aspose.tasks/project/copyto/
---
## CopyTo(Project) {#copyto}

ينسخ البيانات والخصائص الرئيسية للمشروع إلى مشروع آخر.

```csharp
public void CopyTo(Project another)
```

| معامل | النوع | الوصف |
| --- | --- | --- |
| آخر | Project | مشروع آخر لنسخ البيانات إليه. |

## الأمثلة

يعرض كيفية نسخ بيانات المشروع إلى مشروع آخر.

```csharp
var project = new Project(DataDir + "CopyToProjectEmpty.xml");
File.Copy(DataDir + "CopyToProjectEmpty.mpp", DataDir + "ProjectCopying_out.mpp", true);

var mppProject = new Project(DataDir + "ProjectCopying_out.mpp");

// تخطي نسخ بيانات العرض أثناء نسخ بيانات المشروع العامة.
project.CopyTo(mppProject);
```

### انظر أيضًا

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## CopyTo(Project, CopyToOptions) {#copyto_1}

ينسخ البيانات والخصائص الرئيسية للمشروع إلى مشروع آخر.

```csharp
public void CopyTo(Project another, CopyToOptions options)
```

| معامل | النوع | الوصف |
| --- | --- | --- |
| آخر | Project | مشروع آخر لنسخ البيانات إليه. |
| خيارات | CopyToOptions | خيارات النسخ للتحكم في عملية النسخ. |

## الأمثلة

يعرض كيفية نسخ المشروع باستخدام كائن &lt;see cref=\"Aspose.Tasks.CopyToOptions\"/&gt;.

```csharp
var project = new Project(DataDir + "CopyToProjectEmpty.xml");
File.Copy(DataDir + "CopyToProjectEmpty.mpp", OutDir + "ProjectCopying_out.mpp", true);

var mppProject = new Project(OutDir + "ProjectCopying_out.mpp");

// تخطي نسخ بيانات العرض أثناء نسخ بيانات المشروع العامة.
var options = new CopyToOptions
{
    CopyViewData = false
};
project.CopyTo(mppProject, options);
```

### انظر أيضًا

* class [CopyToOptions](../../copytooptions/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


