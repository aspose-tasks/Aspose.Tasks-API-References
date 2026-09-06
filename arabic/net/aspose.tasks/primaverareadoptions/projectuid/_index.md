---
title: "PrimaveraReadOptions.ProjectUid"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية PrimaveraReadOptions. تحصل أو تعيّن UID لمشروع يُقرأ من ملف يحتوي على مشاريع متعددة"
type: docs
weight: 30
url: /ar/net/aspose.tasks/primaverareadoptions/projectuid/
---
## PrimaveraReadOptions.ProjectUid property

يحصل أو يضبط معرف UID لمشروع يُقرأ من ملف يحتوي على مشاريع متعددة.

```csharp
public int ProjectUid { get; set; }
```

## الأمثلة

يظهر كيفية قراءة مشروع من ملف Primavera XML أو Primavera XER يحتوي على مشاريع متعددة.

```csharp
var options = new PrimaveraReadOptions();
options.ProjectUid = 3881;

// يعيد مشروعًا بمعرف UID خاص.
var project = new Project(DataDir + "PrimaveraProject.xml", options);
Console.WriteLine(project.Get(Prj.Name));
```

### انظر أيضًا

* class [PrimaveraReadOptions](../)
* namespace [Aspose.Tasks](../../primaverareadoptions/)
* assembly [Aspose.Tasks](../../../)


