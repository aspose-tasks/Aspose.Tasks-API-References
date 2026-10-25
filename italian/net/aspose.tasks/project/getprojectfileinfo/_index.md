---
title: "Project.GetProjectFileInfo"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Metodo Project. Legge le informazioni del file di progetto dal file"
type: docs
weight: 1280
url: /it/net/aspose.tasks/project/getprojectfileinfo/
---
## GetProjectFileInfo(string) {#getprojectfileinfo_1}

Legge le informazioni del file di progetto dal file.

```csharp
public static ProjectFileInfo GetProjectFileInfo(string filename)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| nomefile | Stringa | Il nome del file del progetto. |

### Valore di ritorno

Le informazioni del file di progetto [`ProjectFileInfo`](../../projectfileinfo/).

## Esempi

Mostra come leggere le informazioni del file di progetto da un file XML.

```csharp
var info = Project.GetProjectFileInfo(DataDir + "Project.xml");
Console.WriteLine("CanRead: " + info.CanRead);
Console.WriteLine("ProjectApplicationInfo: " + info.ProjectApplicationInfo);
Console.WriteLine("ProjectFileFormat: " + info.ProjectFileFormat);
```

### Vedi anche

* class [ProjectFileInfo](../../projectfileinfo/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## GetProjectFileInfo(Stream) {#getprojectfileinfo}

Ottiene le informazioni del file di progetto dallo stream.

```csharp
public static ProjectFileInfo GetProjectFileInfo(Stream stream)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| flusso | Flusso | Il flusso di dati. |

### Valore di ritorno

Le informazioni del file di progetto [`ProjectFileInfo`](../../projectfileinfo/).

## Esempi

Mostra come leggere le informazioni del file di progetto di un file XML letto da un flusso.

```csharp
using (var stream = new FileStream(DataDir + "Project.xml", FileMode.Open))
{
    var info = Project.GetProjectFileInfo(stream);
    Console.WriteLine("CanRead: " + info.CanRead);
    Console.WriteLine("ProjectApplicationInfo: " + info.ProjectApplicationInfo);
    Console.WriteLine("ProjectFileFormat: " + info.ProjectFileFormat);
}
```

### Vedi anche

* class [ProjectFileInfo](../../projectfileinfo/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


