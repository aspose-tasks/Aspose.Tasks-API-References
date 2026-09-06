---
title: "OleObjectCollection.Clear"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Méthode OleObjectCollection. Vide la collection. Afin de persister ces modifications, project.Save doit être appelé avec new MPPSaveOptions  WriteViewData  true"
type: docs
weight: 10
url: /fr/net/aspose.tasks/oleobjectcollection/clear/
---
## OleObjectCollection.Clear method

Efface la collection. Afin de persister ces modifications, project.Save doit être appelé avec new MPPSaveOptions { WriteViewData = true; }

```csharp
public void Clear()
```

## Exemples

Comment vider les objets OLE et persister ces modifications.

```csharp
[C#]
project.OleObjects.Clear();
project.Save("output.mpp", new MPPSaveOptions {WriteViewData = true;} )
```

Montre comment supprimer les objets OLE du projet spécifié.

```csharp
[Test]
public void ClearOleObjects()
{
    var project = new Project(DataDir + "TaskImage2010.mpp");
    project.OleObjects.Clear();
    project.Save(OutDir + "ClearedProject.mpp");
}
```

### Voir aussi

* class [OleObjectCollection](../)
* namespace [Aspose.Tasks](../../oleobjectcollection/)
* assembly [Aspose.Tasks](../../../)


