---
title: "PrimaveraXmlSaveOptions.PrimaveraXmlSaveOptions"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "منشئ PrimaveraXmlSaveOptions. يهيئ مثيلاً جديداً من الفئة PrimaveraXmlSaveOptions"
type: docs
weight: 10
url: /ar/net/aspose.tasks.saving/primaveraxmlsaveoptions/primaveraxmlsaveoptions/
---
## PrimaveraXmlSaveOptions constructor

يهيئ مثيلاً جديداً من الفئة [`PrimaveraXmlSaveOptions`](../).

```csharp
public PrimaveraXmlSaveOptions()
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


