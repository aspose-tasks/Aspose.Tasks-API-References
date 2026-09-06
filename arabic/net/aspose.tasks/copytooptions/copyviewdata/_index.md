---
title: "CopyToOptions.CopyViewData"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية CopyToOptions. تحصل أو تعين قيمة تشير إلى ما إذا كان يجب نسخ بيانات العرض أثناء نسخ بيانات المشروع. القيمة الافتراضية هي true"
type: docs
weight: 20
url: /ar/net/aspose.tasks/copytooptions/copyviewdata/
---
## CopyToOptions.CopyViewData property

يحصل أو يضبط قيمة تشير إلى ما إذا كان يجب نسخ بيانات العرض أثناء نسخ بيانات المشروع. القيمة الافتراضية هي true.

```csharp
public bool CopyViewData { get; set; }
```

## الأمثلة

يظهر كيفية استخدام خيارات نسخ المشروع.

```csharp
var project = new Project(DataDir + "CopyToProjectEmpty.xml");
File.Copy(DataDir + "CopyToProjectEmpty.mpp", OutDir + "ProjectCopying_out.mpp", true);

var mppProject = new Project(OutDir + "ProjectCopying_out.mpp");

// تخطي نسخ بيانات العرض أثناء نسخ بيانات المشروع العامة.
var copyToOptions = new CopyToOptions();
copyToOptions.CopyViewData = false;
project.CopyTo(mppProject, copyToOptions);
```

### انظر أيضًا

* class [CopyToOptions](../)
* namespace [Aspose.Tasks](../../copytooptions/)
* assembly [Aspose.Tasks](../../../)


