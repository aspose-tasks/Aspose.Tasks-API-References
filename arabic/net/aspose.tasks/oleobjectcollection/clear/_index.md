---
title: OleObjectCollection.Clear
second_title: Aspose.Tasks لمرجع .NET API
description: OleObjectCollection طريقة. يمسح المجموعة. من أجل استمرار هذه التغييرات  يجب استدعاء Project.Save باستخدام MPPSaveOptions الجديد WriteViewData  true 
type: docs
weight: 10
url: /ar/net/aspose.tasks/oleobjectcollection/clear/
---
## OleObjectCollection.Clear method

يمسح المجموعة. من أجل استمرار هذه التغييرات ، يجب استدعاء Project.Save باستخدام MPPSaveOptions الجديد {WriteViewData = true؛ }

```csharp
public void Clear()
```

### أمثلة

كيفية مسح كائنات OLE والاستمرار في هذه التغييرات.

```csharp
[C#]
project.OleObjects.Clear();
project.Save("output.mpp", new MPPSaveOptions {WriteViewData = true;} )
```

### أنظر أيضا

* class [OleObjectCollection](../)
* مساحة الاسم [Aspose.Tasks](../../oleobjectcollection/)
* المجسم [Aspose.Tasks](../../../)


