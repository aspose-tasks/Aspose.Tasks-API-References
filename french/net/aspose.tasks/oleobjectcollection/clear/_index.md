---
title: OleObjectCollection.Clear
second_title: Référence de l'API Aspose.Tasks pour .NET
description: OleObjectCollection méthode. Efface la collection. Afin de conserver ces modifications project.Save doit être appelé avec new MPPSaveOptions  WriteViewData  true 
type: docs
weight: 10
url: /fr/net/aspose.tasks/oleobjectcollection/clear/
---
## OleObjectCollection.Clear method

Efface la collection. Afin de conserver ces modifications, project.Save doit être appelé avec new MPPSaveOptions { WriteViewData = true; }

```csharp
public void Clear()
```

### Exemples

Comment effacer les objets OLE et conserver ces modifications.

```csharp
[C#]
project.OleObjects.Clear();
project.Save("output.mpp", new MPPSaveOptions {WriteViewData = true;} )
```

### Voir également

* class [OleObjectCollection](../)
* espace de noms [Aspose.Tasks](../../oleobjectcollection/)
* Assemblée [Aspose.Tasks](../../../)


