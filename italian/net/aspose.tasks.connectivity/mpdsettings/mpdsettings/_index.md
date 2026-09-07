---
title: "MpdSettings.MpdSettings"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Costruttore MpdSettings. Inizializza una nuova istanza della classe MpdSettings."
type: docs
weight: 10
url: /it/net/aspose.tasks.connectivity/mpdsettings/mpdsettings/
---
## MpdSettings constructor

Inizializza una nuova istanza della classe [`MpdSettings`](../).

```csharp
public MpdSettings(string connectionString, int projectId)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| connectionString | Stringa | la stringa di connessione specificata. |
| projectId | Int32 | l'id specificato di un progetto da leggere. |

## Esempi

Mostra come leggere un progetto da un file MPD.

```csharp
DbSettings settings = new MpdSettings("Provider=Microsoft.Jet.OLEDB.4.0; Data Source=" + DataDir + "MpdFileToRead.mpd", 1);
var project = new Project(settings);
Console.WriteLine(project.Get(Prj.Name));
```

### Vedi anche

* class [MpdSettings](../)
* namespace [Aspose.Tasks.Connectivity](../../mpdsettings/)
* assembly [Aspose.Tasks](../../../)


