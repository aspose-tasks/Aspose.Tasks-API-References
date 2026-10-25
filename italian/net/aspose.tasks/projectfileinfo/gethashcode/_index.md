---
title: "ProjectFileInfo.GetHashCode"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Metodo ProjectFileInfo. Restituisce un valore di hash code per l'istanza della classe ProjectFileInfo"
type: docs
weight: 60
url: /it/net/aspose.tasks/projectfileinfo/gethashcode/
---
## ProjectFileInfo.GetHashCode method

Restituisce un valore di hash code per l'istanza della classe [`ProjectFileInfo`](../).

```csharp
public override int GetHashCode()
```

### Valore di ritorno

restituisce un valore di hash per questo oggetto.

## Esempi

Mostra come leggere le informazioni del file di progetto.

```csharp
var info = Project.GetProjectFileInfo(DataDir + "Project.xml");
Console.WriteLine("CanRead: " + info.CanRead);
Console.WriteLine("ProjectApplicationInfo: " + info.ProjectApplicationInfo);
Console.WriteLine("ProjectFileFormat: " + info.ProjectFileFormat);
```

### Vedi anche

* class [ProjectFileInfo](../)
* namespace [Aspose.Tasks](../../projectfileinfo/)
* assembly [Aspose.Tasks](../../../)


