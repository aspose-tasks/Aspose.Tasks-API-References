---
title: OleObjectCollection.Clear
second_title: Aspose.Tasks for .NET API Referansı
description: OleObjectCollection yöntem. Koleksiyonu temizler. Bu değişiklikleri sürdürmek için project.Save yeni MPPSaveOptions  WriteViewData  true 
type: docs
weight: 10
url: /tr/net/aspose.tasks/oleobjectcollection/clear/
---
## OleObjectCollection.Clear method

Koleksiyonu temizler. Bu değişiklikleri sürdürmek için, project.Save, yeni MPPSaveOptions { WriteViewData = true; }

```csharp
public void Clear()
```

### Örnekler

OLE nesneleri nasıl temizlenir ve bu değişikliklere devam edilir.

```csharp
[C#]
project.OleObjects.Clear();
project.Save("output.mpp", new MPPSaveOptions {WriteViewData = true;} )
```

### Ayrıca bakınız

* class [OleObjectCollection](../)
* ad alanı [Aspose.Tasks](../../oleobjectcollection/)
* toplantı [Aspose.Tasks](../../../)


