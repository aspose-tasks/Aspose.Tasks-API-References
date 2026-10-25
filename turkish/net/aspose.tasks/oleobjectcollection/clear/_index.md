---
title: "OleObjectCollection.Clear"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "OleObjectCollection yöntemi. Koleksiyonu temizler. Bu değişiklikleri kalıcı hâle getirmek için project.Save, yeni MPPSaveOptions WriteViewData true ile çağrılmalıdır."
type: docs
weight: 10
url: /tr/net/aspose.tasks/oleobjectcollection/clear/
---
## OleObjectCollection.Clear method

Koleksiyonu temizler. Bu değişiklikleri kalıcı hale getirmek için project.Save, yeni MPPSaveOptions { WriteViewData = true; } ile çağrılmalıdır.

```csharp
public void Clear()
```

## Örnekler

OLE nesnelerini nasıl temizleyip bu değişiklikleri kalıcı hâle getirebilirsiniz.

```csharp
[C#]
project.OleObjects.Clear();
project.Save("output.mpp", new MPPSaveOptions {WriteViewData = true;} )
```

Belirtilen projeden OLE nesnelerini nasıl kaldıracağınızı gösterir.

```csharp
[Test]
public void ClearOleObjects()
{
    var project = new Project(DataDir + "TaskImage2010.mpp");
    project.OleObjects.Clear();
    project.Save(OutDir + "ClearedProject.mpp");
}
```

### Ayrıca Bakınız

* class [OleObjectCollection](../)
* namespace [Aspose.Tasks](../../oleobjectcollection/)
* assembly [Aspose.Tasks](../../../)


