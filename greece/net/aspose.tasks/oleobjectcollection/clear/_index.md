---
title: "OleObjectCollection.Clear"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Μέθοδος OleObjectCollection. Καθαρίζει τη συλλογή. Για να διατηρηθούν αυτές οι αλλαγές, πρέπει να κληθεί το project.Save με νέο MPPSaveOptions  WriteViewData  true"
type: docs
weight: 10
url: /el/net/aspose.tasks/oleobjectcollection/clear/
---
## OleObjectCollection.Clear method

Καθαρίζει τη συλλογή. Για να διατηρηθούν αυτές οι αλλαγές, πρέπει να κληθεί το project.Save με νέο MPPSaveOptions { WriteViewData = true; }

```csharp
public void Clear()
```

## Παραδείγματα

Πώς να καθαρίσετε αντικείμενα OLE και να διατηρήσετε αυτές τις αλλαγές.

```csharp
[C#]
project.OleObjects.Clear();
project.Save("output.mpp", new MPPSaveOptions {WriteViewData = true;} )
```

Δείχνει πώς να αφαιρέσετε αντικείμενα OLE από το καθορισμένο έργο.

```csharp
[Test]
public void ClearOleObjects()
{
    var project = new Project(DataDir + "TaskImage2010.mpp");
    project.OleObjects.Clear();
    project.Save(OutDir + "ClearedProject.mpp");
}
```

### Δείτε επίσης

* class [OleObjectCollection](../)
* namespace [Aspose.Tasks](../../oleobjectcollection/)
* assembly [Aspose.Tasks](../../../)


