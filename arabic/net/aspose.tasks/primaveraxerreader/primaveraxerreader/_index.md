---
title: "PrimaveraXerReader.PrimaveraXerReader"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "منشئ PrimaveraXerReader. يهيئ مثيلاً جديداً من الفئة PrimaveraXerReader"
type: docs
weight: 10
url: /ar/net/aspose.tasks/primaveraxerreader/primaveraxerreader/
---
## PrimaveraXerReader(string) {#constructor_1}

يهيئ مثيلاً جديداً من الفئة [`PrimaveraXerReader`](../).

```csharp
public PrimaveraXerReader(string xerFilePath)
```

| معامل | النوع | الوصف |
| --- | --- | --- |
| xerFilePath | سلسلة | المسار إلى ملف .xer حيث يقع مشروع أو مشاريع Primavera. |

## الأمثلة

يوضح كيفية فحص معلومات المشاريع المختصرة من ملف Primavera XER.

```csharp
var reader = new PrimaveraXerReader(DataDir + "MultiprojectWithExternal.xer");
var projectInfos = reader.GetProjectInfos();
foreach (var info in projectInfos)
{
    Console.WriteLine("{0} - '{1}' - {2}", info.Uid, info.Name, info.ExportFlag);
}

var project = reader.LoadProject(5494);

Console.WriteLine("Loaded project '{0}' with Uid {1}", project.Name, project.Uid);
```

### انظر أيضًا

* class [PrimaveraXerReader](../)
* namespace [Aspose.Tasks](../../primaveraxerreader/)
* assembly [Aspose.Tasks](../../../)

---

## PrimaveraXerReader(Stream) {#constructor}

يهيئ مثيلاً جديداً من الفئة [`PrimaveraXerReader`](../).

```csharp
public PrimaveraXerReader(Stream stream)
```

| معامل | النوع | الوصف |
| --- | --- | --- |
| دفق | دفق | دفق يحتوي على محتوى Primavera XER. |

### انظر أيضًا

* class [PrimaveraXerReader](../)
* namespace [Aspose.Tasks](../../primaveraxerreader/)
* assembly [Aspose.Tasks](../../../)


