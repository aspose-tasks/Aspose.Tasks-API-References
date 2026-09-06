---
title: "PrimaveraXmlSaveOptions.SaveRootTask"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية PrimaveraXmlSaveOptions. تحصل أو تعيين قيمة تشير إلى ما إذا كان سيتم حفظ مهمة الجذر أم لا"
type: docs
weight: 20
url: /ar/net/aspose.tasks.saving/primaveraxmlsaveoptions/saveroottask/
---
## PrimaveraXmlSaveOptions.SaveRootTask property

يحصل أو يعيّن قيمة تشير إلى ما إذا كان سيتم حفظ مهمة جذر أم لا.

```csharp
public bool SaveRootTask { get; set; }
```

## الأمثلة

يظهر كيفية تصدير إلى ملف Primavera XML.

```csharp
var project = new Project(DataDir + "project.xml");

var options = new PrimaveraXmlSaveOptions();
options.SaveRootTask = false;
project.Save(OutDir + "UsingPrimaveraXMLSaveOptions_out.xml", options);
```

### انظر أيضًا

* class [PrimaveraXmlSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../primaveraxmlsaveoptions/)
* assembly [Aspose.Tasks](../../../)


