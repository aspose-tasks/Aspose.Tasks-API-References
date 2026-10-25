---
title: "PrimaveraBaseReader.GetProjectUids"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "طريقة PrimaveraBaseReader. تُرجع قائمة بمعرفات المشاريع الفريدة."
type: docs
weight: 20
url: /ar/net/aspose.tasks/primaverabasereader/getprojectuids/
---
## PrimaveraBaseReader.GetProjectUids method

إرجاع قائمة بمعرفات المشاريع الفريدة.

```csharp
public List<int> GetProjectUids()
```

### قيمة الإرجاع

قائمة بمعرفات المشاريع الفريدة.

## الأمثلة

يعرض كيفية استيراد مشروع من ملف XML الخاص بـ Primavera.

```csharp
var reader = new PrimaveraXmlReader(DataDir + "primavera.xml");
List<int> projectUids = reader.GetProjectUids();
foreach (var projectUid in projectUids)
{
    Console.WriteLine("Project UID: " + projectUid);
}
```

### انظر أيضًا

* class [PrimaveraBaseReader](../)
* namespace [Aspose.Tasks](../../primaverabasereader/)
* assembly [Aspose.Tasks](../../../)


