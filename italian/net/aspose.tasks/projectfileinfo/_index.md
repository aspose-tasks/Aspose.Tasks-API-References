---
title: "Classe ProjectFileInfo"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Classe Aspose.Tasks.ProjectFileInfo. L'istanza della classe contiene informazioni sul formato del file di progetto e sulla versione di Microsoft Project con cui il file è stato creato"
type: docs
weight: 1460
url: /it/net/aspose.tasks/projectfileinfo/
---
## ProjectFileInfo class

L'istanza della classe contiene informazioni sul formato del file di progetto e sulla versione di Microsoft Project con cui il file è stato creato.

```csharp
public sealed class ProjectFileInfo : IEquatable<ProjectFileInfo>
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [CanRead](../../aspose.tasks/projectfileinfo/canread/) { get; } | Restituisce un valore che indica se Aspose.Tasks può elaborare il file di progetto. |
| [IsPasswordProtected](../../aspose.tasks/projectfileinfo/ispasswordprotected/) { get; } | Restituisce un valore che indica se un progetto è protetto da password. |
| [ProjectApplicationInfo](../../aspose.tasks/projectfileinfo/projectapplicationinfo/) { get; } | Restituisce le informazioni sull'applicazione del file di progetto. |
| [ProjectFileFormat](../../aspose.tasks/projectfileinfo/projectfileformat/) { get; } | Restituisce il formato del file di progetto. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| override [Equals](../../aspose.tasks/projectfileinfo/equals/#equals_1)(object) | Restituisce un valore che indica se questa istanza è uguale a un oggetto specificato. |
| [Equals](../../aspose.tasks/projectfileinfo/equals/#equals)(ProjectFileInfo) | Restituisce un valore che indica se questa istanza è uguale a un oggetto specificato. |
| override [GetHashCode](../../aspose.tasks/projectfileinfo/gethashcode/)() | Restituisce un valore di codice hash per l'istanza della classe `ProjectFileInfo`. |

## Osservazioni

Usa la proprietà CanRead per definire che la libreria può elaborare il file di progetto.

## Esempi

Mostra come leggere le informazioni del file di progetto.

```csharp
var info = Project.GetProjectFileInfo(DataDir + "Project.xml");
Console.WriteLine("CanRead: " + info.CanRead);
Console.WriteLine("ProjectApplicationInfo: " + info.ProjectApplicationInfo);
Console.WriteLine("ProjectFileFormat: " + info.ProjectFileFormat);
```

### Vedi anche

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


