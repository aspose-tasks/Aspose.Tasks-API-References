---
title: "ProjectFileInfo.Equals"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Metodo ProjectFileInfo. Restituisce un valore che indica se questa istanza è uguale a un oggetto specificato"
type: docs
weight: 50
url: /it/net/aspose.tasks/projectfileinfo/equals/
---
## Equals(ProjectFileInfo) {#equals}

Restituisce un valore che indica se questa istanza è uguale a un oggetto specificato.

```csharp
public bool Equals(ProjectFileInfo other)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| altro | ProjectFileInfo | L'oggetto specificato da confrontare con questa istanza. |

### Valore di ritorno

Restituisce true se il ProjectFileInfo specificato e questa istanza hanno lo stesso formato file e le stesse informazioni sull'applicazione.

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

---

## Equals(object) {#equals_1}

Restituisce un valore che indica se questa istanza è uguale a un oggetto specificato.

```csharp
public override bool Equals(object obj)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| obj | Oggetto | L'oggetto specificato da confrontare con questa istanza. |

### Valore di ritorno

Restituisce true se il ProjectFileInfo specificato e questa istanza hanno lo stesso formato file e le stesse informazioni sull'applicazione.

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


