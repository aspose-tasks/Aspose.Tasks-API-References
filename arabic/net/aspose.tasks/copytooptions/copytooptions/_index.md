---
title: "CopyToOptions.CopyToOptions"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "منشئ CopyToOptions. يخلق مثيلاً جديدًا لفئة CopyToOptions"
type: docs
weight: 10
url: /ar/net/aspose.tasks/copytooptions/copytooptions/
---
## CopyToOptions constructor

يخلق مثيلاً جديدًا للفئة [`CopyToOptions`](../).

```csharp
public CopyToOptions()
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


