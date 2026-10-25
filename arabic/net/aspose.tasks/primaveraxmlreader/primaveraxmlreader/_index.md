---
title: "PrimaveraXmlReader.PrimaveraXmlReader"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "منشئ PrimaveraXmlReader. يهيئ نسخة جديدة من فئة PrimaveraXmlReader"
type: docs
weight: 10
url: /ar/net/aspose.tasks/primaveraxmlreader/primaveraxmlreader/
---
## PrimaveraXmlReader(string) {#constructor_1}

يُنشئ مثيلاً جديدًا للفئة [`PrimaveraXmlReader`](../).

```csharp
public PrimaveraXmlReader(string templatePath)
```

| معامل | النوع | الوصف |
| --- | --- | --- |
| templatePath | سلسلة | المسار إلى القالب حيث يقع مشروع Primavera Xml أو مشاريع. |

## الأمثلة

يوضح كيفية فحص معلومات المشاريع القصيرة من ملف Primavera XML.

```csharp
var reader = new PrimaveraXmlReader(DataDir + "MultiprojectWithExternal.xml");
var projectInfos = reader.GetProjectInfos();
foreach (var info in projectInfos)
{
    Console.WriteLine("{0} - '{1}' - {2}", info.Uid, info.Name, info.ExportFlag);
}
```

### انظر أيضًا

* class [PrimaveraXmlReader](../)
* namespace [Aspose.Tasks](../../primaveraxmlreader/)
* assembly [Aspose.Tasks](../../../)

---

## PrimaveraXmlReader(Stream) {#constructor}

يُنشئ مثيلاً جديدًا للفئة [`PrimaveraXmlReader`](../).

```csharp
public PrimaveraXmlReader(Stream stream)
```

| معامل | النوع | الوصف |
| --- | --- | --- |
| دفق | دفق | دفق يحتوي على محتوى Primavera Xml. |

## الأمثلة

يوضح كيفية استيراد مشروع من تدفق Primavera XML.

```csharp
using (var stream = new FileStream(DataDir + "primavera.xml", FileMode.Open))
{
    var reader = new PrimaveraXmlReader(stream);
    List<int> projectUids = reader.GetProjectUids();
    foreach (var projectUid in projectUids)
    {
        Console.WriteLine("Project UID: " + projectUid);
    }
}
```

### انظر أيضًا

* class [PrimaveraXmlReader](../)
* namespace [Aspose.Tasks](../../primaveraxmlreader/)
* assembly [Aspose.Tasks](../../../)


