---
title: OleObjectCollection.Clear
second_title: Aspose.Tasks för .NET API-referens
description: OleObjectCollection metod. Rensar samlingen. För att bestå dessa ändringar projekt.Spara bör anropas med nya MPPSaveOptions  WriteViewData  true 
type: docs
weight: 10
url: /sv/net/aspose.tasks/oleobjectcollection/clear/
---
## OleObjectCollection.Clear method

Rensar samlingen. För att bestå dessa ändringar projekt.Spara bör anropas med nya MPPSaveOptions { WriteViewData = true; }

```csharp
public void Clear()
```

### Exempel

Hur man rensar OLE-objekt och behåller dessa ändringar.

```csharp
[C#]
project.OleObjects.Clear();
project.Save("output.mpp", new MPPSaveOptions {WriteViewData = true;} )
```

### Se även

* class [OleObjectCollection](../)
* namnutrymme [Aspose.Tasks](../../oleobjectcollection/)
* hopsättning [Aspose.Tasks](../../../)


