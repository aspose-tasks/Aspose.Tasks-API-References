---
title: "OleObjectCollection.Clear"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "طريقة OleObjectCollection. تُفرغ المجموعة. من أجل حفظ هذه التغييرات يجب استدعاء project.Save مع MPPSaveOptions جديد  WriteViewData  true"
type: docs
weight: 10
url: /ar/net/aspose.tasks/oleobjectcollection/clear/
---
## OleObjectCollection.Clear method

يمسح المجموعة. من أجل حفظ هذه التغييرات يجب استدعاء project.Save مع new MPPSaveOptions { WriteViewData = true; }

```csharp
public void Clear()
```

## الأمثلة

كيفية تفريغ كائنات OLE وحفظ هذه التغييرات.

```csharp
[C#]
project.OleObjects.Clear();
project.Save("output.mpp", new MPPSaveOptions {WriteViewData = true;} )
```

يظهر كيفية إزالة كائنات OLE من المشروع المحدد.

```csharp
[Test]
public void ClearOleObjects()
{
    var project = new Project(DataDir + "TaskImage2010.mpp");
    project.OleObjects.Clear();
    project.Save(OutDir + "ClearedProject.mpp");
}
```

### انظر أيضًا

* class [OleObjectCollection](../)
* namespace [Aspose.Tasks](../../oleobjectcollection/)
* assembly [Aspose.Tasks](../../../)


